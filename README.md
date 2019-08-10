# hass-olibra-icons

Custom icon pack designed for Home Assistant.

## Content

<img src="./svg/bond-logo.svg" width="24" height="24"> bond-logo<br/>


## Install

Copy the html file into `<config>/www/` where `<config>` is your home-assistant config directory (the directory where your `configuration.yaml` resides).

Add the folowing to the `frontend` section of your `configuration.yaml`

```yaml
frontend:
  extra_html_url:
    - /local/hass-olibra-icons.html
```

Restart home-assistant.

## Using

The icons uses the prefix `bha:`.

Example:

```
entities:
  - entity: switch.bond_switch
    icon: 'olibra:bond-logo'
    name: Bond
show_header_toggle: false
type: entities
```

## FAQ

Q: The icon ain't showing, it's just white space where it should be. What's up with that?

A: Probably related to cache. Try opening your instance in a incognito/private Window and see if your icon shows then. If yes, it's cache related. If not, spellcheck.

## Thanks

Thanks to @hulkhaugen for the original [hass-bha-icons](https://github.com/hulkhaugen/hass-bha-icons)
