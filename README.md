# Upload a vagrant box file to Vagrant Cloud

## Prerequisites
- [X] [Vagrant](https://www.vagrantup.com/downloads)

## Instructions

Check on your computer the Vagrant boxes:
```shell
$ vagrant box list
```

```shell
$ vagrant cloud auth login
```

OR

- From [Vagrant Cloud](https://app.vagrantup.com/)
- Go to Settings
- Select Security
- Create an Authentication Token with a Description
- Save the <token>
- Authenticate with the <token>

```shell
$ vagrant cloud auth login --token <token>
```

Upload your local box on VagrantCloud
```shell
$ vagrant cloud publish dlavric/nginx64 1.0.0 Daniela /Users/daniela/Downloads/dlavric/packer-nginx64/nginx64-vbox.box
```

Go on Vagrant Cloud and check the box is uploaded:

https://app.vagrantup.com/dlavric/boxes/nginx64

