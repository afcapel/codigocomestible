require "rubygems"
require "bundler/setup"
require "stringex"

# This will be configured for you when you run config_deploy
deploy_branch  = "master"

## -- Misc Configs -- ##

public_dir      = ""    # compiled site directory
source_dir      = "."    # source file directory
blog_index_dir  = '.'    # directory for your blog's index page (if you put your index in source/blog/index.html, set this to 'source/blog')
new_post_ext    = "markdown"  # default new post file extension when using the new_post task
new_page_ext    = "markdown"  # default new page file extension when using the new_page task
server_port     = "4000"      # port for preview server eg. localhost:4000

#######################
# Working with Jekyll #
#######################

desc "Generate jekyll site"
task :generate do
  puts "## Generating Site with Jekyll"
  system "compass compile --css-dir #{source_dir}/stylesheets"
  system "jekyll"
end

desc "Watch the site and regenerate when it changes"
task :watch do
  puts "Starting to watch source with Jekyll and Compass."
  system "compass compile --css-dir ./stylesheets --sass-dir ./_sass"
  jekyllPid = Process.spawn("jekyll --server --auto")
  compassPid = Process.spawn("compass watch")

  trap("INT") {
    [jekyllPid, compassPid].each { |pid| Process.kill(9, pid) rescue Errno::ESRCH }
    exit 0
  }

  [jekyllPid, compassPid].each { |pid| Process.wait(pid) }
end

desc "preview the site in a web browser"
task :preview do
  puts "Starting to watch source with Jekyll and Compass. Starting Rack on port #{server_port}"
  jekyllPid = Process.spawn("jekyll --server --auto")
  compassPid = Process.spawn("compass watch")

  trap("INT") {
    [jekyllPid, compassPid].each { |pid| Process.kill(9, pid) rescue Errno::ESRCH }
    exit 0
  }

  [jekyllPid, compassPid].each { |pid| Process.wait(pid) }
end
