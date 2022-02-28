#### Build and tag an image
```
docker build . -t rails_docker
```

#### Run a tagged image in a container interactively
The bundle exec command is needed to tell your computer when you want to run a command using a gem from the current application’s Gemfile.

```
docker run -it -p 3000:3000 rails_docker bundle exec rails server -b 0.0.0.0 -p 3000
```