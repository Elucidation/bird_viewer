# Birb overview

I have a camera that tracks and captures small crop images of motion objects including birds.
It sees several types of birds (crows, juncos, finches, sparrows etc.) which I'd like to classify.

```json
[
    {"area":null,
    "box":null,
    "camera":"birbcam",
    "end_time":1704213300.999055,
    "false_positive":null,
    "has_clip":true,
    "has_snapshot":true,
    "id":"1704213243.00595-x47jwu",
    "label":"bird",
    "plus_id":null,
    "ratio":null,
    "region":null,
    "retain_indefinitely":false,
    "start_time":1704213238.00595,
    "sub_label":null,
    "top_score":0.82421875,
    "zones":[],
    "thumbnail":"<base64 encoded image>"},
    // ... more entries 
]

```

The camera provides the cropped images and associated metadata as an events JSON data file.
First, lets make a webpage that can load this JSON events file and do some simple visualizations.

![Example page](example_page.jpg)


## Running

`python -m http.server`