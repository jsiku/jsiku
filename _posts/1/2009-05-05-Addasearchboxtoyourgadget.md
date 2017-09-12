---
layout : post
title: 가젯에 검색창달기
date: '2009-05-05 14:03:00 +0900'
author: Siku
published: true
tags: 검색창
---
<ul>
<li>sns.jsiku.com(폐쇄)에서 옮김</li>
</ul>
<a href="http://blogger.jsiku.com/2009/05/blogger-navbar.html">navbar를 제거</a>하면 블로그 내의 검색기능을 활용할 수 없는데, 이에 많은 불편을 느끼실 것입니다. 가젯을 검색하여도 찾기가 어려운데 직접 코드를 입력하여 가젯을 추가하는 방법이 있습니다.

가젯 추가에서 HTML/Javascript에서 다음과 같은 코드를 입력하면 됩니다.

&lt;form id="searchThis" action="/search" style="display:inline;" method="get"&gt;&lt;input id="searchBox" name="q" type="text"/&gt; &lt;input id="searchButton" value="Find" type="submit"/&gt;&lt;/form&gt;
<div></div>
<div>위의 코드에서 value 값을 수정하면 박스, 버튼, 텍스트 등의 양식등을 변경할 수 있습니다.</div>

