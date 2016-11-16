# Atmosphere Guides

This repo contains multiple guides that are hosted on Github Pages:
[https://cyverse.github.io/atmosphere-guides](https://cyverse.github.io/atmosphere-guides).

## Guides Overview

### User Guide

This guide will explain how Atmosphere works from the perspective of the End
User. (Don't mention Troposphere or other jargon for the End User).

### Staff Guide

This guide will explain how Atmosphere works from the perspective of a Staff
user (With Admin privileges)

### Imaging Guide

This guide will contain handy information for End Users looking to create new
images.

## How to Contribute

### How to Write Docs
Guides are written in Markdown. You may want to use a tool to render your Markdown. [livedown](https://github.com/shime/livedown) works with a few editors to hot-load your changes.

Here is another tool to make nice GIFs.
http://recordit.co/

### How to Compile Docs
After making changes, you need to compile them (so they will show up in GitHub Pages).

First, you must have [pandoc](http://pandoc.org/) installed and in your executable path -- see [Installing Pandoc](http://pandoc.org/installing.html).

If you create a new guide, you will also need to update the Makefile so that `to_html_template.sh` builds HTML for your new guide.

Finally, to compile the docs, run `make` from the root of this repository.

See CONTRIBUTING.md for Pandoc-specific details not covered here.

### Notice for CyVerse Documenters
A lot of Atmosphere documentation lives on the [CyVerse Wiki](https://pods.iplantcollaborative.org/wiki/dashboard.action), some in the [Atmosphere Manual](https://pods.iplantcollaborative.org/wiki/display/atmman/Atmosphere+Manual+Table+of+Contents) and some in private spaces. Going forward, documentation should be maintained as follows:

- Docs for Atmosphere(1) as *the open-source platform for cloud computing* should be hosted here on [atmosphere-guides](https://cyverse.github.io/atmosphere-guides), and what exists on the CyVerse wiki should be migrated here.
- Docs for Atmosphere(0) as *CyVerse's cloud computing service for bioscience research* should remain on the CyVerse wiki, in [Atmosphere Manual](https://pods.iplantcollaborative.org/wiki/display/atmman/Atmosphere+Manual+Table+of+Contents) or other spaces as appropriate.

When you do migrate content from the CyVerse wiki to atmosphere-guides, please *remove the content from the wiki* and *leave a link to the new guide in its place*. This way, we avoid maintaining parallel documentation on multiple platforms, while helping others find information in its new location.
