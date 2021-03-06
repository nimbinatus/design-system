---
title: Alert Bar
parent: Notifications
layout: component
category: Components
usage: >
  A notification bar extends fully across the top of an content container within a Helix interface in order to provide the user with feedback relating to the status of the item. It can be scoped across the entirety of the content area (page level scoping) or scoped to extend across a singular section of the content area (element level scoping).
preview-image: preview-images/alert-bar.svg
status: stable
resource: true
last-modified: 2017-08-17
helix-ui-css: true
helix-ui-javascript: true
pagelink: https://rackerlabs.github.io/helix-ui/components/alerts/
---

{% include toc.html %}

<section class="static-section" markdown="1">

## Introduction

<div class="hxRow"  markdown="1">
{% column left:"hxCol hxSpan-12-xs hxSpan-12-sm hxSpan-4-md hxSpan-4-lg" %}

An alert bar can extend across the entirety of the content area (page level scoping) or across a singular section of the content area (element level scoping).

### When to Use

- Notification bars are best used for information that will remain static, barring user intervention. For example, an informative message surrounding a new feature being made available to a user.
- For information that is more ephemeral and fleeting, we recommend using another notification type.

### Best Practices

- Ensure notification bars have implicit priority based on the alert type from most to least severity level: Error > Warning > Success > Informational
- Ensure notification bars are used sparingly and limited to one per page.
- For multiple alert bars, stack them in order of criticality, high-to-low, top-to-bottom.

{% endcolumn %}

{% column right:"hxCol hxSpan-12-xs hxSpan-12-sm hxSpan-8-md hxSpan-8-lg" %}
{% figure [caption:"Page level scoping example"] [class:"image bg-light border"] %}
 <embed src="{{site.url}}/assets/images/components/content-areas/alerts/alert-bar-hero.svg"/>
{% endfigure %}
{% endcolumn %}
</div>

</section>

<section class="static-section" markdown="1">

## Design Specs

<div class="hxRow"  markdown="1">
{% column left:"hxCol hxSpan-12-xs hxSpan-12-sm hxSpan-4-md hxSpan-4-lg" %}

### Composition

The alert bar pattern is comprised of six parts. Three required, three
optional:

- Alert bar containing element (required) — Holds all other elements and displays the status color.
- Status icon (required) — Acts as supporting information to the status color.
- Alert description (required) — Describes to the user why the alert bar exists.
- Alert type (optional) — An optional alert title descriptor.
- Alert action link (optional) — Provides a user with the next step of a process.
- Close action (optional) — Closes the alert.

{% endcolumn %}

{% column right:"hxCol hxSpan-12-xs hxSpan-12-sm hxSpan-8-md hxSpan-8-lg" %}
{% figure [caption:"Alert bar composition"] [class:"image bg-light border"] %}
 <embed src="{{site.url}}/assets/images/components/content-areas/alerts/alert-bar-composition.png" width="617"/>
{% endfigure %}

{% figure [caption:"Alert bar specifications."] [class:"image bg-light border"] %}
 <embed src="{{site.url}}/assets/images/components/content-areas/alerts/alert-bar-specs.png" width="617"/>
{% endfigure %}
{% endcolumn %}
</div>

</section>

<section class="static-section" markdown="1">

<div class="hxRow"  markdown="1">
{% column left:"hxCol hxSpan-12-xs hxSpan-12-sm hxSpan-4-md hxSpan-4-lg" %}

### Multi-line alerts

Alert messages should be as concise and clear as possible. We recommend keeping to a limit of 140-160 characters. Following this rule will keep an alert message as a single-line comment (at Desktop and Wall breakpoints). In instances where text wrapping is needed, it will follow the behavior shown in the illustration.

{% endcolumn %}

{% column right:"hxCol hxSpan-12-xs hxSpan-12-sm hxSpan-8-md hxSpan-8-lg" %}
{% figure [caption:"Multiline alert wrapping behavior"] [class:"image bg-light border"] %}
 <embed src="{{site.url}}/assets/images/components/content-areas/alerts/alert-bar-multiline-alerts.png" width="617"/>
{% endfigure %}
{% endcolumn %}
</div>

</section>

<section class="static-section" markdown="1">

<div class="hxRow"  markdown="1">
{% column left:"hxCol hxSpan-12-xs hxSpan-12-sm hxSpan-4-md hxSpan-4-lg" %}

### Status types

The alert bar pattern enables users to assess status of a given section at a glance. This pattern supports four statuses:

{% endcolumn %}

{% column right:"hxCol hxSpan-12-xs hxSpan-12-sm hxSpan-8-md hxSpan-8-lg" %}
{% figure [caption:"Alert bar status types."] [class:"image bg-light border"] %}
 <embed src="{{site.url}}/assets/images/components/content-areas/alerts/alert-bar-status-types.png" width="617px"/>
{% endfigure %}
{% endcolumn %}
</div>

</section>
