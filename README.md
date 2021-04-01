building personal site

adding certain lines to parsa css: go into `/assets/css/style.css` (maybe in theme, but preferably in top level?)

meant to allow images to be moved within text
```
img[src$='#center']
{
    display: block;
    margin: 0.7rem auto; /* you can replace the vertical '0.7rem' by
                            whatever floats your boat, but keep the
                            horizontal 'auto' for this to work */
    /* whatever else styles you fancy here */
}

img[src$='#floatleft']
{
    float:left;
    margin: 0.7rem;      /* this margin is totally up to you */
    /* whatever else styles you fancy here */
}

img[src$='#floatright']
{
    float:right;
    margin: 0.7rem;      /* this margin is totally up to you */
    /* whatever else styles you fancy here */
}
```

styling of bullets, change `ol,ul` stuff:
```
ul {
 list-style-type: disc;
 margin: 0px;
}
```

adding academic icons:
- downloaded [academicons](https://github.com/jpswalsh/academicons/archive/v1.9.1.zip) zip
- put the fonts folder and `academicons.css` into `.../themes/parsa/static/plugins/academic-icons/`
- added these lines to my `config.toml`:
```
[[params.plugins.css]]
link = "plugins/academic-icons/academicons.css"
```



To get head "featured" image in "featured" pages to be left justified, normal size, go to `/themes/parsa/layouts/_default/single.html`. For the `regular page`, change img line attributes: `class="img-fluid rounded float-left mr-5 mb-4"`. (probably could do this better by adding another page type, but)
