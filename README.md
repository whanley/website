building personal site

adding certain lines to parsa css:

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
