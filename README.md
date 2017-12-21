# AskOmics Website

AskOmics website is available at [https://askomics.github.io](https://askomics.github.io). It is automaticaly build from the master branch of this repository.

## Run on your own computer

### Dependancies

```bash
sudo apt install -y ruby ruby-dev
sudo gem install jekyll bundler
```

### Run

```bash
cd askomics.github.io
bundle install # Only the first time
bundle exec jekyll serve
```
Website well be available at [localhost:4000](http://localhost:4000)
