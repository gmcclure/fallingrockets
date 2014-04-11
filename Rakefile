task :default => [:deploy]

desc "Deploy the site"
task :deploy do
  sh "jekyll build"
  sh "rsync -avz --delete _site/ tsm:/var/www/clients/fallingrockets"
end

desc "Serve and watch"
task :s do
  sh "jekyll serve --watch"
end
