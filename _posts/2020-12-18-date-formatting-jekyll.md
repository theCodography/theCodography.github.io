---
title: Date formatting Jekyll
layout: post
date: 2020-12-18T04:12:00Z
description: Định dạng ngày tháng có thể phức tạp nếu bạn cần một định dạng cụ thể. Trong bài viết này, mình sẽ chỉ cho bạn cách tạo ngày tháng ở hầu hết mọi định dạng.
imgUrl: jekyll.jpg
---
## Giới thiệu
Định dạng ngày tháng có thể phức tạp nếu bạn cần một định dạng cụ thể. Trong bài viết này, mình sẽ chỉ cho bạn cách tạo ngày tháng ở hầu hết mọi định dạng.

## Setup
Chúng ta sẽ bắt đầu bằng cách đặt ngày ở ISO 8601 format.
<pre class='highlight'>
<code>---
layout: default
title: Date Formatting
date: 2016-03-23T10:20:00Z
---</code>
</pre>
Bây giờ chúng ta có thể chạy input qua 1 filter để có được định dạng mong muốn.

## date_to_long_string
Input:
<pre class='highlight'><code>&#123;&#123; page.date | date_to_long_string &#125;&#125;</code></pre>
Output:
<pre class='highlight'>23 March 2016</pre>

## date_to_rfc822
Input:
<pre class='highlight'><code>&#123;&#123; page.date | date_to_rfc822 &#125;&#125;</code></pre>
Output:
<pre class='highlight'>Wed, 23 Mar 2016 23:20:00 +1300</pre>

## date_to_string
Input:
<pre class='highlight'><code>&#123;&#123; page.date | date_to_string &#125;&#125;</code></pre>
Output:
<pre class='highlight'>23 Mar 2016</pre>

## date_to_xmlschema
Input:
<pre class='highlight'><code>&#123;&#123; page.date | date_to_xmlschema &#125;&#125;</code></pre>
Output:
<pre class='highlight'>2016-03-23T23:20:00+13:00</pre>

## date
<span class ='highlight'>date</span> cho phép chúng ta kiểm soát toàn bộ định dạng. Chúng ta có thể chỉ định một định dạng cụ thể mà chúng ta mong muốn. Ví dụ:

Input:
<pre class='highlight'><code>&#123;&#123; page.date | date: "%m/%d/%Y" &#125;&#125;</code></pre>
Output:
<pre class='highlight'>03/23/2016</pre>
or

Input:
<pre class='highlight'><code>&#123;&#123; page.date | date: "%-d %B %Y" &#125;&#125;</code></pre>
Output:
<pre class='highlight'>23 March 2016</pre>

