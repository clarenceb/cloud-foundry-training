Cloud Foundry Training VM
=========================

Virtual Machine for working on the Cloud Foundry Training.

Setup (Mac OS X)
----------------

### Prerequisites:

* Install the [Homebrew](http://brew.sh/) package manager
* Install [Homebrew Cask](https://caskroom.github.io/) to be able to install binary applications via Homebrew
* Install VirtualBox:

```sh
brew cask install virtualbox
```

* Install Vagrant:

```sh
brew cask install vagrant
```

* Install Ansible:

```sh
brew install ansible
```

* (Optional) Install [Vagrant Cachier](http://fgrehm.viewdocs.io/vagrant-cachier/) plugin:

```sh
vagrant plugin install vagrant-cachier
```

Provisioning the VM
-------------------

```sh
vagrant up
```

SSH into the VM:

```sh
vagrant ssh
```

Shared folders
--------------

The folder `/vagrant` is shared between the host machine (where this repo is cloned) and the Virtual Machine.

Tools included in the VM
------------------------

* Oracle JDK 8
* Cloud Foundry CLI (`cf`)
* Git (`git`)
* Maven (`mvn`)

Tools you'll need to install yourself on your host
--------------------------------------------------

* A web browser: Chrome or Firefox
* (Optional) Web browser plugins: "Asciidoctor.js Live Preview" and "JSONView"
* (Optional) An IDE or Editor of your choice (e.g. Spring Tool Suite (STS), Eclipse, Intellij, Atom, SublimeText, vim, etc.)
  * To install STS: `brew cask install sts`
  * To install Eclipse JEE edition: `brew cask install eclipse-jee`
  * To install IntelliJ IDEA: `brew cask install intellij-idea`
  * To install Atom: `brew cask install atom`
  * To install Sublime Text 2: `brew cask install sublime-text`
