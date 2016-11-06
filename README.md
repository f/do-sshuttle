# DO-sshuttle

Transparent your Proxy your connection over your DigitalOcean Droplet.

## Installation

### 1. Install Requirements

```sh
# Install DigitalOcean CLI Tool
brew install doctl

# Install sshuttle
brew install sshuttle
```

### 2. Generate DigitalOcean API Key

Generate a key from [https://cloud.digitalocean.com/settings/api/tokens](https://cloud.digitalocean.com/settings/api/tokens)

### 3. Login via `doctl`

```sh
doctl auth login
# Enter your API key you generated.
```

### 4. Create a Droplet called `do-sshuttle-server`

Create a Droplet on your DigitalOcean account. Name it `do-sshuttle-server`.

### 5. Start Proxying.

```sh
$ ./do-sshuttle
do-shuttle v0.0.1
Fatih Kadir Akın <fatihkadirakin@gmail.com>
Transparent Proxying over DigitalOcean Droplets

[ds] <--- Getting do-sshuttle-server Droplet information...
[ds] ---> Powering on do-sshuttle-server (root@<IP ADDRESS>) Droplet...
[ds] ---> Power-on Request sent...
[ds] ---> Allow server 10 seconds to boot...
[ds] ---> Proxying network via sshuttle...
client: Connected.
```

## LICENSE

WTFPL.
