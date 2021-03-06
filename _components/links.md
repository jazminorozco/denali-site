---
title: 'Links'
permalink: /documentation/components/links
excerpt: 'Links connect pages to each other and allow users to perform actions within a page. They come in a variety of sizes and styles and can be used together with icons.'
---

# {{ page.title }}
{{ page.excerpt }}


***


### Links
Implement links by wrapping text in an `<a>` tag.

{% capture link_default %}{% highlight html %}
<a>Click Here</a>
{% endhighlight %}{% endcapture %}
{% include code-snippet.html code=link_default url='link_default.html' %}

### States
Links have active and disabled states. An active state is triggered when a link is clicked or hovered. It can be forced by adding the `.is-active` class to a link&#39;s `<a>` tag. Conversely, a disabled state can be implemented by adding the `.is-disabled` class to a link&#39;s `<a>` tag.

{% capture link_states %}{% highlight html %}
<a>Default Link</a>
<a class="is-active">Active or Hovered Link</a>
<a class="is-disabled">Disabled Link</a>
{% endhighlight %}{% endcapture %}
{% include code-snippet.html code=link_states url='link_states.html' %}

### Small links
Small sized links can be implemented by adding the `.is-small` class to a link&#39;s `<a>` tag.

{% capture link_sizes %}{% highlight html %}
<a>Default Link</a>
<a class="is-small">Small Link</a>
{% endhighlight %}{% endcapture %}
{% include code-snippet.html code=link_sizes url='link_sizes.html' %}


***


### Links with icons
Icons can be used as links, either on their own or accompanied by text. To add an icon to a link insert an `<i>`tag with the `.d-icon` and `.d-$icon-name` classes within the `<a>` tag.

#### Front
To place an icon at the front of a link add `.has-icon-front` to the `<a>` tag.

{% capture link_icons_front %}{% highlight html %}
<a class="has-icon-front"><i class="d-icon d-add-circle"></i>Default size with icon in front</a>
<br>
<a class="is-small has-icon-front"><i class="d-icon d-add-circle"></i>Small size with icon in front</a>
{% endhighlight %}{% endcapture %}
{% include code-snippet.html code=link_icons_front url='link_icons_front.html' %}

#### Back
To place an icon to the back of a link add `.has-icon-back` to the `<a>` tag.

{% capture link_icons_back %}{% highlight html %}
<a  class="has-icon-back">Default size with icon<i class="d-icon d-external is-sub"></i></a>
<br>
<a class="is-small has-icon-back">Small size with icon<i class="d-icon d-external is-sub"></i></a>
{% endhighlight %}{% endcapture %}
{% include code-snippet.html code=link_icons_back url='link_icons_back.html' %}


***


### Secondary
Secondary links are grey in color. To create a secondary link add the `.is-secondary` class to an `<a>` tag.

{% capture link_secondary %}{% highlight html %}
<a class="is-secondary">Secondary Link</a>
{% endhighlight %}{% endcapture %}
{% include code-snippet.html code=link_secondary url='link_secondary.html' %}


***


### Sub action
Sub action links can be blue or grey in color but appear a lower opacity. To create a sub action link add the `.is-sub` class to an `<a>` tag.

{% capture link_sub %}{% highlight html %}
<a class="is-sub">Sub Link</a>
<br>
<a class="is-secondary is-sub">Secondary Sub Link</a>
{% endhighlight %}{% endcapture %}
{% include code-snippet.html code=link_sub url='link_sub.html' %}


***


### Variables
You can use these variables to customize this component. Simply set one or multiple of these variables and recompile the SCSS.

`$link-config:`

|**Name**|**Type**|**Default value**|**Computed value**|
|`text-color`                  |color     |`map-get($denali-brand-colors, '600')`             |#3697f2           |
|`hover-text-color`            |color     |`map-get($denali-brand-colors, '700')`             |#3570f4           |
|`disabled-text-color`         |color     |`rgba(map-get($denali-grey-colors, '800'), .2)`    |rgba(#303030, .2) |
|`secondary:text-color`        |color     |`map-get($denali-grey-colors, '700')`              |#606060           |
|`secondary:hover-text-color`  |color     |`map-get($denali-grey-colors, '800')`              |#303030           |
|`inverse:text-color`          |color     |`map-get($denali-grey-colors, '100')`              |#fffff            |
|`inverse:hover-text-color`    |color     |`rgba(map-get($denali-grey-colors, '100'), .4)`    |rgba(#ffffff, .4) |
|`small:text-size`             |font-size |`1.2rem`                                           |12px              |
