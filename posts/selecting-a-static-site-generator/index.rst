.. title: Selecting a static site generator
.. slug: selecting-a-static-site-generator
.. date: 2021-11-02 22:15:18 UTC+01:00
.. status: draft
.. tags: tag1,tag2,tag3
.. category: meta
.. link: 
.. description: 
.. type: text

There are many problems associated with writing a blog - finding the time to update it regularly, finding an audience, engaging said audience so they return, fend off spam in the comments section - to name only a few. But the problems start even before that:

What platform do I use? Which commenting system do I use? Do I need statistics on page views etc?

It was clear from the beginning that I want to keep my site clean and lean. Using a static site generator sounded like a good idea. But which one to use? and what even is this thing?

Static Site Generators
----------------------

A static site generator generates static files, easy as pie. But ... what is the alternative?

In modern CMS systems like Wordpress or Joomla, all content is saved in a database. Whenever a page is requested, the contents are assembled from from various parts of that database. The header and footer are in one place, the text in another, and meta data - data about the text - in yet another place. When your browser requests to see this page, the server as to go and find all the bits and pieces, put them all together, and then send the result to your browser for you to see. When you come back to the page another time, the page will be assembled all over again.[1] These sites are called dynamic.

Static sites, in contrast, are saved as HTML files. Each page is its own file, and it contains everything that is needed to display it - text, images, title, header and footer, a menu - everything is in one, static file. It is assembled once, before uploading it to the server. When your browser requests it from the server, it can be sent back immediately.

Just as with CMS systems, there are a lot of static site generators around. Which one to choose?

