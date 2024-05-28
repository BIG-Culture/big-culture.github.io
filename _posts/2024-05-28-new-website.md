---
layout: post
title: BIG-Culture Website Goes Live
date: 2024-05-28 15:13:13
description: Our new website is now live at big-culture.github.io
tags: website_updates
categories: sample-posts
tabs: true
giscus_comments: true
---

This is how a post with [tabs](https://github.com/Ovski4/jekyll-tabs) looks like. Note that the tabs could be used for different purposes, not only for code.

## First tabs

To add tabs, use the following syntax:

{% raw %}

```liquid
{% tabs group-name %}

{% tab group-name tab-name-1 %}

Content 1

{% endtab %}

{% tab group-name tab-name-2 %}

Content 2

{% endtab %}

{% endtabs %}
```

{% endraw %}

With this you can generate visualizations like:

{% tabs log %}

{% tab log php %}

```php
var_dump('hello');
```

{% endtab %}

{% tab log js %}

```javascript
console.log("hello");
```

{% endtab %}

{% tab log ruby %}

```javascript
pputs 'hello'
```

{% endtab %}

{% endtabs %}

## Another example

{% tabs data-struct %}

{% tab data-struct yaml %}

```yaml
hello:
  - "whatsup"
  - "hi"
```

{% endtab %}

{% tab data-struct json %}

```json
{
  "hello": ["whatsup", "hi"]
}
```

{% endtab %}

{% endtabs %}

## Tabs for something else

{% tabs something-else %}

{% tab something-else text %}

Regular text

{% endtab %}

{% tab something-else quote %}

> A quote

{% endtab %}

{% tab something-else list %}

Hipster list

- brunch
- fixie
- raybans
- messenger bag

{% endtab %}

{% endtabs %}
