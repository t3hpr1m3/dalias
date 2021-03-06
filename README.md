# dalias
[![Gitlab pipeline status (self-hosted)](https://img.shields.io/gitlab/pipeline/dubzland/dalias/main?gitlab_url=https%3A%2F%2Fgit.dubzland.net)](https://git.dubzland.net/dubzland/dalias/pipelines)
[![Liberapay patrons](https://img.shields.io/liberapay/patrons/jdubz)](https://liberapay.com/jdubz/donate)
[![Liberapay receiving](https://img.shields.io/liberapay/receives/jdubz)](https://liberapay.com/jdubz/donate)

Dynamic bash aliases (loosely based on [rbenv](https://github.com/rbenv/rbenv)).

## Installation
The simplest method is a git checkout:
```sh
$ git checkout https://github.com/t3hpr1m3/dalias.git ~/.dalias
$ echo 'export PATH="$HOME/.dalias/bin:$PATH"' >> ~/.bash_profile
$ echo 'eval $(dalias init)' >> ~/.bash_profile
```

You will need to restart your shell for the above to take effect.

## Usage
Usage is fairly straightforward.  Navigate to a directory where you wish to add an alias.  Let's say that in this directory, you want to run rspec within your Docker container (via docker-compose):
```sh
$ dalias add rspec docker-compose run app bundle exec rspec
```

## License
*dalias* is released under the [MIT License](LICENSE).
