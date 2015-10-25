squarespace-blocks
==================

> Which blocks can you customize and how to go about doing so.



## About
This is simply a repository of Squarespace template block override files for all the blocks that you can currently override. Following is a list of which blocks are unlocked and which ones are off limits.



## How
To override a Squarespace system block, add a `[system-block-name].block` file and a `[system-block-name].block.conf` file in your `blocks` directory. The actual block name you need to use to do this can be found when inspecting the block node in the browser in it's `className` string. For instance, the `image` block has this class: `sqs-block image-block sqs-block-image` and thus the override `type` is `image`.



#### Unlocked
- quote
- image
- audio
- gallery ( grid, slider, slideshow, stacked )
- summary-v2 ( autocolumns, carousel, list, autogrid )
- form
- newsletter
- menu
- calendar?
- tourdates? ( brandsintown? )
- opentable?
- search
- collectionlink
- button
- tagcloud
- archive
- donate?
- chart ( bar, line, pie )
- socialaccountlinks-v2
- rss



#### Locked
- text
- markdown
- video
- album / playlist
- embed
- spacer
- horizontalrule
- map
- code
- product
- amazon
- twitter
- foursquare
- fivehundredpix
- instagram
- flickr
- soundcloud