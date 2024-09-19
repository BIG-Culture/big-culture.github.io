---
layout: page
title: Pete Bennett
description: Lecturer, interested in playful interfaces, tangible interaction and generative music.
img: assets/img/people/bennett.gif
importance: 1
category: academics #academics, associates, or students
related_publications: true
---

[www.peteinfo.com](https://www.peteinfo.com)

<script>
  const feedUrl = 'https://research-information.bris.ac.uk/en/persons/peter-d-bennett/projects/?format=rss';  // Change to the actual RSS feed URL
  
  let parser = new RSSParser();

  parser.parseURL(feedUrl, function(err, feed) {
    if (err) {
      console.error("RSS feed error:", err);
      return;
    }
    
    let feedContent = '';
    feed.items.forEach(function(entry) {
      feedContent += '<h3><a href="' + entry.link + '">' + entry.title + '</a></h3>';
      feedContent += '<p>' + entry.contentSnippet + '</p>';
    });
    document.getElementById('rss-feed').innerHTML = feedContent;
  });
</script>
