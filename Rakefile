task :default => :serve

desc "Run a local web server"
task :serve do
  sh "python -m SimpleHTTPServer"
end

desc "Publish to github pages"
task :publish do
  sh "git checkout gh-pages"
  sh "git rebase master"
  sh "git push origin gh-pages"
  sh "git checkout master"
end

desc "Synchronise with github repository"
task :push do
  sh "git push origin master"
end