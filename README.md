squarespace-blocks
==================

> Which blocks can you customize and how to go about doing so.



### About
This is simply a repository of Squarespace template block override files for all the blocks that you can currently override. Following is a list of which blocks are unlocked and which ones are off limits.



### How
To override a Squarespace system block, add a `[system-block-name].block` file and a `[system-block-name].block.conf` file in your `blocks` directory. The actual block name you need to use to do this can be found when inspecting the block node in the browser in it's `className` string. For instance, the `image` block has this class: `sqs-block image-block sqs-block-image` and thus the override `type` is `image`.



### Noteworthy
Not all system blocks can be overriden as easily as others. For instance, several require a hefty amount of javascript to render the system block. When overriding these blocks, you can get a variety of behavior. Overriding the `chart` block would require you to do your own charting with the data provided. The `calendar` block renders your override template, but Squarespace javascript still executes and loads the calendar into the container. The `opentable` and `tourdates` blocks integrate with third-party services. The ability to override blocks is powerful and cool, even though you cannot do this for all your favorite blocks, like `soundcloud`! A great man once said, "With great power comes great responsibility."

Enjoy playing around and making your Squarespace sites even more unique but just remember to be conscious about what you're doing. For instance, if you're building a site for a client, **make sure you still support all the CMS options in your custom block render**! All the data is there, so you can do it very easily. But choosing a 2up grid gallery with 40px of spacing and not getting it would be frustrating. But, if you're doing something else and you're cool with not accounting for the CMS options, that's cool too. Awareness is really all that matters here.



### Blocks
A quick note about the `blocks`. I did my best to comment each block and they even include notes on the data that is passed to that block template. It still helps to run the block with the `console.log` to better inspect the data you are working with in Chrome. But that data references are a good starting point. Also, if you are using block overrides with the [node-squarespace-server](https://github.com/NodeSquarespace/node-squarespace-server), you have to push the templates up to your site in order to see them render locally as well. This is due to the fact that the blocks are used to render the `mainContent` or `body` of pages and collection items.



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
