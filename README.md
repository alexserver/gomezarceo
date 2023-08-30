# gomezarceo
www.gomezarceo.mx hugo content


## Prerrequisites

### Install Hugo

- MacOs

```
brew install hugo
```

[installation docs](https://gohugo.io/installation/)


## Quickstart

### Run Hugo Web Server

```
$hugo server
```

### Build Web Site

```
$hugo
```

## Create new content

```
$hugo new content [path]/document.md
```

## Web server deploy in gomezarceo.mx

The web server is in a DigitalOcean Ubuntu 16.04 droplet
What I do to deploy is

1. Commit my changes, and push to github
2. Enter to my droplet through SSH
3. Enter to my apache domain directory for `gomezarceo.mx`
4. Run `hugo` to build the static website into `[website_path]/public`

### Troubleshot

If you need to update hugo, it's only about downloading the latest release (Download the Hugo Extended version)
from [here](https://github.com/gohugoio/hugo/releases/tag/v0.117.0)

```
$wget https://github.com/gohugoio/hugo/releases/download/v0.117.0/hugo_extended_0.117.0_Linux-64bit.tar.gz
$cp hugo /usr/bin/
```

and that's it, it should good to go