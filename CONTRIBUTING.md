# Contributing

Welcome to All Hands Active's source code for our website!

This document will help teach you how to contribute to our website.
Thank you for helping us make our website better!

- [Contributing](#contributing)
  - [Installing dependencies](#installing-dependencies)
    - [Using a dev container](#using-a-dev-container)
    - [Manual Installation](#manual-installation)
      - [Installing Ruby](#installing-ruby)
        - [Installing without asdf](#installing-without-asdf)
      - [Installing ruby gems](#installing-ruby-gems)
  - [Running the site](#running-the-site)
  - [Making changes](#making-changes)
    - [Pushing changes upstream](#pushing-changes-upstream)
  - [Thanks for contributing](#thanks-for-contributing)

## Installing dependencies

> [!Warning]
> If you are on Fedora 42, there are issues conflicting with Ruby and compiling gems with native extensions. One possible workaround is to downgrade your C compiler. Another alternative is to use dev containers.
>
> See <https://github.com/rbenv/ruby-build/wiki#fedora-42-and-ruby-31> for more information.

### Using a dev container

We have a [dev container](https://containers.dev/) configured in order to make contributing easier. If you have an [editor that supports dev containers](https://containers.dev/supporting#editors), you can simply start up our container to automatically enter an environment with all dependencies.

The source code and configuration for our devcontainer is located in [.devcontainer](.devcontainer).

Please note this option requires Docker to be installed and running.

Once the dev container is up and running, you can skip ahead to running the site.

### Manual Installation

#### Installing Ruby

We recommend one of the toolchain managers, like `asdf`, `mise`, `RVM`, or `rbenv`.

`asdf` and `mise` are useful for managing multiple toolchains, such as Javascript, Python, and Ruby, whereas `RVM` and `rbenv` manage _only_ Ruby installations.

If you do not already have `asdf` installed, go ahead and do so. Then return to this guide.

1\. Add the ruby plugin to `asdf`.

```sh
asdf plugin add ruby https://github.com/asdf-vm/asdf-ruby.git
```

2\. Install ruby.

```sh
asdf install
```

##### Installing without asdf

See [the official ruby documentation](https://www.ruby-lang.org/en/documentation/installation/) for the best ways to install Ruby.

> [!NOTE]
> Whichever method you pick, make sure you install ruby **3.2.2**.
> This is the version we use for building our website. This is why we recommend using a version manager such as `asdf` or `RVM`

#### Installing ruby gems

Now that our Ruby installation exists, we can use `bundle` to install our ruby gems.

```sh
bundle install
```

If this command errors out, check that you have a valid `gcc` compiler on your path, and install one if you don't.

## Running the site

Now that our dev environment has our dependencies installed, we can go ahead and start up the jekyll dev server.

```sh
bundle exec jekyll serve
```

This will start a jekyll development server which will watch for any edits to our website, and automatically reload the backend.

Please note that jekyll will not automatically reload the frontend, so you'll need to manually refresh the browser to see any changes.

## Making changes

> [!Warning]
>
> BEFORE starting work on an issue, please make sure that there is an open issue for your change, and that someone else is not already working on it.
> We hate seeing contributions go to waste as multiple people were working on it.
>
> Please comment on an issue letting us know you want to work on it before starting work on it!

> [!Tip]
> If you are new to using GitHub and Git in general, check out the guides on Github that explain how to use Git and work with others on projects using Git!
>
> <https://github.com/git-guides>

If this is your first time contributing to our website, [create a fork](https://github.com/allhandsactive/site/fork) before making any changes. This is where you will push your commits.

Next, create a new branch with

```sh
git branch -c <feat/<NAME_OF_CHANGE>
```

Try to name it something descriptive, like a branch for creating a contributing document would be named feat/add-contributing.md


### Pushing changes upstream

When you are satisfied with your changes, commit to a new branch (not the master branch!) and push it to a fork on GitHub.

From there, [create a pull request](https://github.com/allhandsactive/site/pull/new) and fill out the form there.

## Thanks for contributing

If you encounter any issues setting up an enviroment or have any questions, please let us know by [opening an issue](https://github.com/allhandsactive/site/issues/new).
