https://www.flickr.com/photos/warl0rd/4476784615/in/photolist-7PAG6D-YmsHrH-TuLMHn-5p75wv-Y6jqEu-Y93Ks2-2bU3e5Q-SWTWza-VKu15s-ZsxJXR-2bU3eeh-28EYNHk-K24wDg-SvS9C9-Tz95Uc-Yj3A85-Lx8Syw-27i3i8z-LYoLu6-297zbAe-2c2AQH6-Ngtqzg-PTBkvj-2aJqkTT-28EYPTr-25UVomu-27i31v6-K23LJn-PNy87G-Ux3H6s-24C6USj-2azPZAD-NdmPoV-Lx9dC9-27iHqvE-YwwpBo-27zukyY-K24t2g-KeSZs1-2aSyue9-YDNS2J-Ndop9t-UzHErY-Sk9igr-25UVpfJ-Ux3QSE-2azTtYK-26h2FXC-2azT5uk-Xfn21A

# Reveal.js webpack starter

Another webpack starter for reveal.js

## Usage

Clone this proyect and change the **./content** directory:

* Edit _config.json_

* Add slides and index them on config.json (glob patterns supported!)

* Add your media files to be added on the bundle.

* Edit your custom css on _content/css/index.scss_.

* plugins are conditionally added to the bundle:

```json
{
  "title": "🦄 Irontec reveal.js - webpack starter demo 🦄",
  "options": {
    "controls": true,
    "progress": true,
    "history": true,
    "center": true,
    "slideNumber": false,
    "touch": true,
    "hideAddressBar": true,
    "mouseWheel": true
  },
  "plugins": {
    "search": true,
    "zoom":   true,
    "menu":   true,
    "notes":  true,
    "highlightjs": true
  },
  "slides": [
    {"path": "index.md", "attrs": {"class":"intro"}},
    [
        "subcontent/*.md"
    ],
    "end.html"
  ]
}
```


## Development time


```bash
npm start
```

Will open a dev-server on http://localhost:8080


## Bundle time

```bash
npm run build
```

Will create a build on _./dist/_.


# TODO

* npm init command
* ¿Auto publish on github/gitlab pages?
* generate a SEO friendly dist



