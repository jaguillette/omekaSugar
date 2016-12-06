---
layout: post
title:  "Bring in Image-Based Maps through Web Map Services"
date:   2016-10-11 14:28:19 -0400
categories: tutorial collections
---

Neatline allows you to bring in georeferenced image data from other servers
through WMS or Web Map Service. Some collections allow data to be embedded in
this way, and if they do, you can layer those maps on top of a modern map in
Neatline.

To add a WMS layer to a Neatline record, you just have to add the URL for your
map and its title into the record's style, like so:

![image of WMS Address and WMS Layer Name entered into Neatline.](https://s3.amazonaws.com/dh-general-purpose/wms_info.png)

The hard part is getting that URL from your data source. This tutorial will show
how to embed a map from Harvard's Map Warper (or the New York Public Library
version of the same program), so that you can use a map that you've
georeferenced yourself using Map Warper, or one in the site's collections that
has already been georeferenced.

In Map Warper, select a map, then go to the Export tab. There, you'll see a
number of export options. You want the "WMS base URL". There is a separate link
on the text "for JOSM OpenStreetMap Editor", so make sure that you get the URL
from "WMS base URL". Just right click that text, and click "Copy link address"
(which might have slightly different phrasing, depending on your browser).

![image showing right click on WMS base URL](https://s3.amazonaws.com/dh-general-purpose/wms_right_click.png)

That's the URL that you'll paste in to your Neatline record, under "WMS url".
You'll also need the title of the map. The map in this example is called "1893
Chicago Midway", so that's what we'll past into "WMS layer name"

![image of WMS Address and WMS Layer Name entered into Neatline.](https://s3.amazonaws.com/dh-general-purpose/wms_info.png)

You can set the opacity of the map by setting "Fill Opacity" and "Fill Opacity
Selected", also under style.

Other sites also serve their maps as WMS, but they show those links in different
ways. In any case, you'll need a url, as well as the layer title. Take a look at
the WMS url you just copied in. If another site gives you a similar-looking url,
then there's a good chance it'll work.

Some things that I run into when testing out these layers:
* Especially for maps at a small scale, they won't show up until you're looking
right at them, and Neatline may not zoom to them. Find out where your map is,
and see if it's where it should be.
* The default fill opacity for a record in Neatline is 0.3 (only 30% opaque), so
your map will probably be very faint when you first load it. If you're having a
hard time seeing it, bump the opacity up to 1 (100% opaque).
* Double check that you've copied the right url. It should look something like
http://warp.worldmap.harvard.edu/maps/wms/14, which you'll notice is short and
has "wms" in it.

If there are specific sites that you'd like to see covered in this tutorial,
you can [submit an issue on this site's GitHub repo](https://github.com/jaguillette/omekaSugar/issues),
or [email the author](mailto:jguillette@fas.harvard.edu). No guarantees it'll
happen, but it's also likely that you're not the only one with this problem. We
might as well figure it out together.
