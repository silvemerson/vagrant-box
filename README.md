# Custom Vagrant box with Packer

## Installing Packer

### Add the HashiCorp GPG key.

```curl -fsSL https://apt.releases.hashicorp.com/gpg | sudo apt-key add -```

### Add the official HashiCorp Linux repository.

```sudo apt-add-repository "deb [arch=amd64] https://apt.releases.hashicorp.com $(lsb_release -cs) main"```

### Update and install

```sudo apt-get update && sudo apt-get install packer```

## Building

```packer build file_name.pkr.json```

## Configuring Vagrant

```vagrant box add NAME_BOX output-vagrant/package.box```


