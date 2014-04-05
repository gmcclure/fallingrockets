task :default => [:deploy]

task :deploy do
  sh "jekyll build"
  sh "rsync -avz --delete _site/ tsm:/var/www/clients/fallingrockets"
end

task :s do
  sh "jekyll serve --watch"
end
