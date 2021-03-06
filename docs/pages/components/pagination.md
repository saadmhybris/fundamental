---
title: Pagination
keywords: pagination
sidebar: left-navigation-sidebar
toc: false
permalink: pagination.html
folder: components
summary:
---

Use pagination components in conjunction with Tables (recommended) or Cards (if needed) to allow for more efficient performance and quick access to specific records in the overall data set.

<hr>

## First Page
When the first page is active, the previous link should be disabled.

{% capture pagination %}
<ul class="fd-pagination">
    <span class="fd-pagination__total">30 items</span>
    <li class="fd-pagination__item fd-pagination__item--previous">
        <button class="fd-button fd-button--text fd-button--icon fd-button--small" aria-label="Previous" aria-disabled="true">
            <span class="fd-icon fd-icon--chevron fd-icon--small" role="presentation"></span>
        </button>
    </li>
    <li class="fd-pagination__item">
        <a href="#" class="fd-pagination__link" aria-selected="true">1</a>
    </li>
    <li class="fd-pagination__item">
        <a href="#" class="fd-pagination__link">2</a>
    </li>
    <li class="fd-pagination__item">
        <a href="#" class="fd-pagination__link">3</a>
    </li>
    <li class="fd-pagination__item">
        <button class="fd-button fd-button--text fd-button--icon fd-button--small" aria-label="Next">
            <span class="fd-icon fd-icon--chevron fd-icon--small" role="presentation"></span>
        </button>
    </li>
</ul>
{% endcapture %}

{% include display-component.html component=pagination %}

<br>

## Second Page
Example with second page active.

{% capture pagination-second %}
<ul class="fd-pagination">
    <span class="fd-pagination__total">30 items</span>
    <li class="fd-pagination__item fd-pagination__item--previous">
        <button class="fd-button fd-button--text fd-button--icon fd-button--small" aria-label="Previous" aria-disabled="true">
            <span class="fd-icon fd-icon--chevron fd-icon--small" role="presentation"></span>
        </button>
    </li>
    <li class="fd-pagination__item">
            <a href="#" class="fd-pagination__link">1</a>
    </li>
    <li class="fd-pagination__item">
            <a href="#" class="fd-pagination__link" aria-selected="true">2</a>
    </li>
    <li class="fd-pagination__item">
            <a href="#" class="fd-pagination__link">3</a>
    </li>
    <li class="fd-pagination__item">
        <button class="fd-button fd-button--text fd-button--icon fd-button--small" aria-label="Next">
            <span class="fd-icon fd-icon--chevron fd-icon--small" role="presentation"></span>
        </button>
    </li>
</ul>
{% endcapture %}

{% include display-component.html component=pagination-second %}

<br>

## More than three Pages

{% capture pagination-more %}
<ul class="fd-pagination">
    <span class="fd-pagination__total">500 items</span>
    <li class="fd-pagination__item fd-pagination__item--previous">
        <button class="fd-button fd-button--text fd-button--icon fd-button--small" aria-label="Previous" aria-disabled="true">
            <span class="fd-icon fd-icon--chevron fd-icon--small" role="presentation"></span>
        </button>
    </li>
    <li class="fd-pagination__item">
            <a href="#" class="fd-pagination__link">1</a>
    </li>
    <li class="fd-pagination__item">
            <a href="#" class="fd-pagination__link" aria-selected="true">2</a>
    </li>
    <li class="fd-pagination__item">
            <a href="#" class="fd-pagination__link">3</a>
    </li>
    <li class="fd-pagination__item">
    <span class="fd-pagination__more"
        aria-hidden="true"
        aria-label="..."
        role="presentation">&#8226;&#8226;&#8226;</span>
    </li>
    <li class="fd-pagination__item">
            <a href="#" class="fd-pagination__link">50</a>
    </li>
    <li class="fd-pagination__item">
        <button class="fd-button fd-button--text fd-button--icon fd-button--small" aria-label="Next">
            <span class="fd-icon fd-icon--chevron fd-icon--small" role="presentation"></span>
        </button>
    </li>
</ul>
{% endcapture %}

{% include display-component.html component=pagination-more %}

<br>

## In between more than three Pages

{% capture pagination-more-between %}
<ul class="fd-pagination">
    <span class="fd-pagination__total">500 items</span>
    <li class="fd-pagination__item fd-pagination__item--previous">
        <button class="fd-button fd-button--text fd-button--icon fd-button--small" aria-label="Previous" aria-disabled="true">
            <span class="fd-icon fd-icon--chevron fd-icon--small" role="presentation"></span>
        </button>
    </li>
    <li class="fd-pagination__item">
        <a href="#" class="fd-pagination__link">1</a>
    </li>
    <li class="fd-pagination__item">
        <span class="fd-pagination__more"
            aria-hidden="true"
            aria-label="..."
            role="presentation">&#8226;&#8226;&#8226;</span>
    </li>
    <li class="fd-pagination__item">
        <a href="#" class="fd-pagination__link">21</a>
    </li>
    <li class="fd-pagination__item">
        <a href="#" class="fd-pagination__link" aria-selected="true">22</a>
    </li>
    <li class="fd-pagination__item">
        <a href="#" class="fd-pagination__link">23</a>
    </li>
    <li class="fd-pagination__item">
        <span class="fd-pagination__more"
            aria-hidden="true"
            aria-label="..."
            role="presentation">&#8226;&#8226;&#8226;</span>
    </li>
    <li class="fd-pagination__item">
            <a href="#" class="fd-pagination__link">50</a>
    </li>
    <li class="fd-pagination__item">
        <button class="fd-button fd-button--text fd-button--icon fd-button--small" aria-label="Next">
            <span class="fd-icon fd-icon--chevron fd-icon--small" role="presentation"></span>
        </button>
    </li>
</ul>
{% endcapture %}

{% include display-component.html component=pagination-more-between %}

<br>

## Last Page
On the last page, the next link should be disabled.

{% capture pagination-last %}
<ul class="fd-pagination">
    <span class="fd-pagination__total">500 items</span>
    <li class="fd-pagination__item fd-pagination__item--previous">
        <button class="fd-button fd-button--text fd-button--icon fd-button--small" aria-label="Previous" aria-disabled="true">
            <span class="fd-icon fd-icon--chevron fd-icon--small" role="presentation"></span>
        </button>
    </li>
    <li class="fd-pagination__item">
        <a href="#" class="fd-pagination__link">1</a>
    </li>
    <li class="fd-pagination__item">
        <span class="fd-pagination__more"
            aria-hidden="true"
            aria-label="..."
            role="presentation">&#8226;&#8226;&#8226;</span>
    </li>
        <li class="fd-pagination__item">
            <a href="#" class="fd-pagination__link">49</a>
        </li>
    <li class="fd-pagination__item">
            <a href="#" class="fd-pagination__link" aria-selected="true">50</a>
    </li>
    <li class="fd-pagination__item">
        <button class="fd-button fd-button--text fd-button--icon fd-button--small" aria-label="Next">
            <span class="fd-icon fd-icon--chevron fd-icon--small" role="presentation"></span>
        </button>
    </li>
</ul>
{% endcapture %}

{% include display-component.html component=pagination-last %}
