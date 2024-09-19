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

<div id="rss-feed"></div>

<!-- RSS Parser Library -->
<script src="https://cdn.jsdelivr.net/npm/rss-parser/dist/rss-parser.min.js"></script>

<!-- RSS Feed Fetching and Display Script -->
<script>
  document.addEventListener("DOMContentLoaded", function() {
    const feedUrl = 'https://research-information.bris.ac.uk/en/persons/peter-d-bennett/projects/?format=rssl';
    
    let parser = new RSSParser();
    
    // Fetch and display the RSS feed
    parser.parseURL(feedUrl, function(err, feed) {
      if (err) {
        console.error("Error fetching RSS feed:", err);
        return;
      }
      
      let feedContent = '';
      feed.items.forEach(function(entry) {
        feedContent += '<h3><a href="' + entry.link + '">' + entry.title + '</a></h3>';
        feedContent += '<p>' + entry.contentSnippet + '</p>';
      });

      // Inject the RSS content into the rss-feed div
      document.getElementById('rss-feed').innerHTML = feedContent;
    });
  });
</script>