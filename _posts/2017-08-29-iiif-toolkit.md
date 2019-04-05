---
layout: post
title:  "Use IIIF Toolkit for Zoomable, Annotatable Images"
date:   2017-08-29 09:00:00 -0400
categories: tutorial iiif
---

The International Image Interoperability Framework (IIIF) is a standard for serving images over the web that provides a way for a variety of tools to use images made available with the standard. It's fundamental infrastructure for rich media sharing.

The [IIIF Toolkit](https://github.com/utlib/IiifItems) is an Omeka plugin developed at the University of Toronto to make it easy to use IIIF content within Omeka.

In practical terms, that means that the plugin lets you use images from any repository that supports IIIF, so you get beautiful, archival quality scans in a modern interface, with annotation capabilities to boot.

Importing a IIIF image requires a IIIF manifest. Where you can find this manifest depends on the repository, but if there's a IIIF option that gives you a URL, that's usually it.

For example, in the LUNA browser that the David Rumsey Map Collection uses, you can find a IIIF manifest URL here:

![Image showing location of IIIF URL in David Rumsey Collection, under share, then IIIF](https://s3.amazonaws.com/dh-general-purpose/Screen+Shot+2017-08-29+at+10.33.29+AM.png)

Again, where you find this URL will vary from repository to repository, and some repositories won't support IIIF yet. However, there is a list of sites that implement IIIF in this "[IIIF Awesome](https://github.com/IIIF/awesome-iiif#implementations)" repository.

One thing to be aware of is that a IIIF manifest may represent many images. You could be interested in a page from a book, and get the manifest for the whole book. What each manifest represents depends on the repository, so just be aware that you might get more than you bargained for.

Once you have a repository with URLs you can get, you can import those materials into Omeka. The form in IIIF Toolkit is pretty easy to use at that point. You can specify the size of the preview image that you want. I use 512 x 512, but you may find a more restrictive repository that limits you to 96 x 96, or you may want smaller images for larger manifests.

![Image of IIIF Toolkit import form, with Type -> Manifest, Source -> URL, and the David Rumsey URL entered](https://s3.amazonaws.com/dh-general-purpose/Screen+Shot+2017-08-29+at+10.34.18+AM.png)

When you click "Import", you'll be taken to a progress page, and see the status of the import. This is also when you'll see if your import starts bringing in every page of a 500 page manuscript. We'll go into how to undo that later.

When the import completes, you will have a new item for each image represented in the manifest, and a new collection that brings together all of the images in the manifest.

If you find that you've imported more than you've bargained for, you can run a search for items sourced to the IIIF manifest, and delete them all via the search results page there.

<div style='position:relative; padding-bottom:calc(57.06% + 44px)'><iframe src='https://gfycat.com/ifr/MaleInformalKookaburra?autoplay=0&controls=1&hd=1' frameborder='0' scrolling='no' width='100%' height='100%' style='position:absolute;top:0;left:0;' allowfullscreen></iframe></div><p> <a href="https://gfycat.com/MaleInformalKookaburra">via Gfycat</a></p>

<script type="text/javascript" src="https://assets.gfycat.com/gfycat.js"></script>
