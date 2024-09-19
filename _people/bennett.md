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
    const feedUrl = 'https://research-information.bris.ac.uk/en/persons/peter-d-bennett/projects/?format=rss';  // Replace with actual RSS feed URL
    const corsProxy = 'https://api.rss2json.com/v1/api.json?rss_url='; // Use a public CORS proxy

    let parser = new RSSParser();

    // Fetch and display the RSS feed
    parser.parseURL(corsProxy + encodeURIComponent(feedUrl), function(err, feed) {
      if (err) {
        console.error("Error fetching RSS feed:", err);
        return;
      }

      let feedContent = '';
      feed.items.forEach(function(entry) {
        let entryLink = entry.link.trim();  // Clean up the link in case of any unwanted spaces
        feedContent += '<h3><a href="' + entryLink + '" target="_blank" rel="noopener noreferrer">' + entry.title + '</a></h3>';
        feedContent += '<p>' + entry.contentSnippet + '</p>';
      });

      // Inject the RSS content into the rss-feed div
      document.getElementById('rss-feed').innerHTML = feedContent;
    });
  });
</script>
