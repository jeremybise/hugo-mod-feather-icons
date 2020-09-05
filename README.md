Feather icons available as a Hugo module.

Feather is a collection of simply beautiful open source icons. Each icon is designed on a 24x24 grid with an emphasis on simplicity, consistency, and flexibility. See https://github.com/feathericons/feather

## Use

Import the module into your Hugo project's site config:

```toml
[[module.imports]]
path = "github.com/jeremybise/hugo-mod-feather-icons"
```

The icons gets mounted in `assets/svg/feather`.

This means that they can be used like this in a Hugo template:

```html
{{ $icon := resources.Get "feathericons/search.svg" }} {{ $icon.Content |
safeHTML }}
```

Or, use the shortcode:

```html
{{ partial "feathericons/icon" "arrow-up-right" }}
```

See https://github.com/feathericons/feather/tree/master/icons for a full list of icons.
