# Software Security Tools Demo

This is a compilation of Software Security tools for demos and talks about them
for developers.

# Requirements

The following are the requisites for each tool. These can be used independently
of each other. Enclosed in parentheses is the version of the tool in which I
tested the tools against, not the minimal requirement.

* Java (8) and Maven (3.3)
* Ruby via RVM (1.27.0)
* Node.js via [NVM](https://github.com/creationix/nvm) (6.2.1)

# Instructions for use

Clone the repo:

```shell
git clone https://github.com/injcristianrojas/swsec_tools_demo.git
cd swsec_tools_demo
git submodule update --init --recursive
```

## Java

Go to `swsec_tools_demo/swsec-intro-java` and run `mvn site`.

## Ruby

If you have RVM installed, go to `swsec_tools_demo`. Ruby gemset and version are
configured. If you don't have the required Ruby version, RVM will alert saying
something like `ruby-X.X.X is not installed`. Install it using
`rvm install ruby-X.X.X`. After that, install the corresponding gems:

```shell
gem install bundler
bundle install
```

## Node.js

If you have NVM installed, go to `swsec_tools_demo`. Run `nvm use`. If you don't
have the reqiured Node and npm versions, NVM will alert with something like
`version "vX.X.X" is not yet installed`. Install it using `nvm install vX.X.X`.
After that, install the corresponding modules:

```shell
npm install -g retire nsp snyk
```
