tags: #webhook #server #CD #go 
# webhook
[webhook](https://github.com/adnanh/webhook) is a lightweight configurable tool written in Go, that allows you to easily create HTTP endpoints (hooks) on your server, which you can use to execute configured commands. You can also pass data from the HTTP request (such as headers, payload or query variables) to your commands. [webhook](https://github.com/adnanh/webhook) also allows you to specify rules which have to be satisfied in order for the hook to be triggered.

## Installation

### Building from source

To get started, first make sure you've properly set up your [Go](http://golang.org/doc/install) 1.14 or newer environment and then run

$ go build github.com/adnanh/webhook

to build the latest version of the [webhook](https://github.com/adnanh/webhook).

### Using package manager

#### Snap store

[![Get it from the Snap Store](https://camo.githubusercontent.com/353bcf397acd2a7663c45bc69cd2b202417a66c24d3b38f861f9cc0fe1a25324/68747470733a2f2f736e617063726166742e696f2f7374617469632f696d616765732f6261646765732f656e2f736e61702d73746f72652d77686974652e737667)](https://snapcraft.io/webhook)

#### Ubuntu
If you are using Ubuntu linux (17.04 or later), you can install webhook using `sudo apt-get install webhook` which will install community packaged version.

#### Debian
If you are using Debian linux ("stretch" or later), you can install webhook using `sudo apt-get install webhook` which will install community packaged version (thanks [@freeekanayaka](https://github.com/freeekanayaka)) from [https://packages.debian.org/sid/webhook](https://packages.debian.org/sid/webhook)

### Download prebuilt binaries

Prebuilt binaries for different architectures are available at [GitHub Releases](https://github.com/adnanh/webhook/releases).

## Usage
Describe config file:
```json
[
  {
    "id": "redeploy-webhook",
    "execute-command": "/var/scripts/redeploy.sh",
    "command-working-directory": "/var/webhook"
  }
]
```

Run:
```bash
/path/to/webhook -hooks hooks.json -verbose
```

It will start up on default port 9000 and will provide you with one HTTP endpoint
http://yourserver:9000/hooks/redeploy-webhook

## Links
**Documentation**: [github](https://github.com/adnanh/webhook)