# From: https://github.com/ainc/awesomeinc2013/blob/master/Rakefile 

require "rubygems"
require "tmpdir"

require "bundler/setup"
require "jekyll"

ENV["JEKYLL_ENV"] = "production"

desc "Generate blog files"
task :generate do
  Jekyll::Site.new(Jekyll.configuration({
    "source"      => ".",
    "destination" => "_site"
  })).process
end


desc "Generate and publish site to gh-pages"
task :publish => [:generate] do
  Dir.mktmpdir do |tmp|
    cp_r "_site/.", tmp

    pwd = Dir.pwd
    Dir.chdir tmp

    system "git init"
    system "git add ."
    message = "Site updated at #{Time.now.utc}"
    system "git commit -m #{message.inspect}"
    system "git branch master"
    system "git checkout master"
    system "git branch"
    system "git remote add orgin https://github.com/JRD971000/JRD971000.github.io"
    system "git push orgin master --force"

    Dir.chdir pwd
  end
end
