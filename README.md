The files for the CONTINENTS webpage.

# To develop locally

Install Ruby: https://www.ruby-lang.org/en/documentation/installation/

Change gem install location, add to `~/.bash_rc` or equivalent:

```bash
export GEM_HOME="$HOME/.gems"
export PATH="$HOME/.gems/bin:$PATH"
```

Install Bundler:

```bash
gem install bundler
```

Install the gems in the repo:

```bash
bundler install
```

Build website:

```bash
bundler exec jekyll serve
```
