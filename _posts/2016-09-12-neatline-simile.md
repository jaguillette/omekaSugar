---
layout: post
title:  "Make a Map + Timeline with Neatline Simile"
date:   2016-09-12 10:23:11 -0400
categories: tutorial collections
---

Neatline Simile is a plugin for Neatline, which is itself a plugin for Omeka, that allows you to tell stories about the items in your Omeka site using maps and timelines. It does this by associating things on a map with periods of time, which show up on a timeline at the bottom of the map.

Note that I'm assuming that you have the Neatline and Neatline Simile plugins on your site and installed. If you don't, you'll need to either [add it to your site yourself](https://omeka.org/codex/Managing_Plugins_2.0), or contact your site administrator to get them to install it. Here's where you'll find out:

<div class="gfycontainer"><div class='gfyitem' data-id='UntimelyAchingAmericanindianhorse' data-autoplay='false' data-responsive='true'></div></div>

Once you're sure you have the plugins installed, you need to enable the plugin for your Neatline Exhibit. I'm assuming that you've already set one up, but if you haven't, you may want to look at [a previous post on setting up a Neatline exhibit]({% post_url 2016-09-07-make-a-neatline-exhibit %}).

<div class="gfycontainer"><div class='gfyitem' data-id='FearlessBriskFlyingsquirrel' data-autoplay='false' data-responsive='true'></div></div>

You'll want to set up your timeline to focus on a time appropriate to your story, and to use an appropriate time scale. To do this, you'll need to check out the options for it on your exhibit, and set them to a center and scale that makes sense. Interval pixels, track height, and tape height are all related to how your timeline will display, and are measured in pixels. Here's what they all do, from [the Neatline Simile Documentation](http://docs.neatline.org/working-with-the-simile-timeline-widget.html):

![Simile timeline display parameters](http://neatline.org/wp-content/uploads/2014/05/timelinedefs.png)

And here's where you'll find all of those options:

<div class="gfycontainer"><div class='gfyitem' data-id='UnimportantBouncyHummingbird' data-autoplay='false' data-responsive='true'></div></div>

You'll need to enable the Simile widget for each Neatline Record that you want to have show up on your timeline.

<div class="gfycontainer"><div class='gfyitem' data-id='FatherlyShrillDowitcher' data-autoplay='false' data-responsive='true'></div></div>

Then you'll need to set the date parameters for that record. There are two different date parameters. Start and End dates control where the Record displays on the timeline. You can just set a Start Date to make a record show up as a single point on the timeline, or both for a span of time.

<div class="gfycontainer"><div class='gfyitem' data-id='ActiveOldfashionedBlacklab' data-autoplay='false' data-responsive='true'></div></div>

Before and After dates control when the map geometry for the Record will display as a user moves through the timeline.

<div class="gfycontainer"><div class='gfyitem' data-id='PeriodicWindingGreyhounddog' data-autoplay='false' data-responsive='true'></div></div>

Now you have a Record in your Neatline Exhibit that also shows up on a timeline. Just as you can click on the map geometry for a record to bring up its description, you can click on a timeline segment to do the same thing.

<script type="text/javascript" src="https://assets.gfycat.com/gfycat.js"></script>
