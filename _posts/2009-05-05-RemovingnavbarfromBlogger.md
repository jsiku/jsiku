---
layout : post
title: Blogger에서 navbar의 제거
date: '2009-05-05 09:49:00 +0900'
author: Siku
published: true
tags: navbar 제거
---
<ul>
<li>sns.jsiku.com(폐쇄)에서 옮김</li>
</ul>
blogger 도움말에서 navbar의 제거를 치면 정말 많은 글들이 올라와 있습니다.. 많은 사람들이 이러한 navbar를 제거하고 싶어하는데, 아마 각자의 디자인과 맞지 않아 거부감 때문에 그럴 것입니다. navbar는 레이아웃의 HTML편집에서 다음과 같은 코드를 CSS 부분에 삽입하면 제거됩니다.
<blockquote>#navbar, #navbar-iframe {
height: 0px;
visibility: hidden;
display: none;
}</blockquote>
이런 navbar를 제거하면 블로그내 검색기능을 사용할 수 없는데, 가젯을 찾아보아도 검색창은 찾을 수가 없었습니다. 좀 더 검색해본 결과 가젯의 코드를 삽입하는 방식이 있는데 <a href="http://blogger.jsiku.com/2009/05/blog-post.html">여기서</a> 확인할 수 있습니다.

