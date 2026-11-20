# Me & Family

A multi-page family photo site. Its separate HTML pages make it a useful example of keeping navigation, assets and visual styling consistent across a small static website.

[Open the live demo](https://oniseg.github.io/MeFamily/) · [View screenshot](https://raw.githubusercontent.com/onisEg/resume/23df91e50f87b60e1360d79edcc24cf77eb09b07/public/projects/my-family.webp)

## Site tour

1. Start at the homepage, which introduces the family and contains a Recent Photos carousel. That widget loads jQuery and Owl Carousel from external CDNs.
2. Follow the story, events and gallery links to separate documents under the pages directory. File names are case-sensitive on GitHub Pages.
3. The contact page contains name, email, subject and message fields. Its form has an empty action and this repository contains the frontend presentation.

## Run locally

From the repository root, serve the checked-in files with Python 3:

```sh
python -m http.server 8000
```

Open [localhost:8000](http://localhost:8000/) to load `index.html`. The browser reads the HTML, styles and assets directly. On Windows, `py -m http.server 8000` starts the same server.

## Source guide

| File or directory | What to look for |
| --- | --- |
| [index.html](index.html) | Home page, recent photos and carousel dependencies. |
| [pages/story.html](pages/story.html) | Family story page. |
| [pages/Events.html](pages/Events.html) | Events page. |
| [pages/Gallery.html](pages/Gallery.html) | Gallery page. |
| [pages/contact.html](pages/contact.html) | Contact form layout. |
| [css/style.css](css/style.css) | Shared page styling. |

## Manual walkthrough

Navigate from the homepage to Gallery and back, then load the gallery URL directly. Check that the images still resolve from the nested directory. If Recent Photos is static, inspect the CDN script requests on the homepage.
