---
layout : post
title: 다수의 컴퓨터를 하나의 컴퓨터로... Synergy+
date: '2009-10-21 11:43:11 +0900'
author: Siku
published: true
tags: 컴퓨터
---
Aion을 하고 싶어서 노트북에 설치했더니..
사양의 한계로 설치하지 못하였습니다.

(이런…)

그래서 집에서 사용하는 데스크탑을 연구실로 가지고 왔습니다.
아이온은 약 한달만 사용하고. 그 다음부터는 흥미가 떨어져 하지 않았는데.

맨 아래의 사진에서 보는 것 처럼 은폐된 위치에서 동영상 및 각종 컨텐츠만을 소비하는 행위만 하고 오른쪽의 노트북에서 실제 연구와 관련된 작업은 전혀 이루어지지 못하게 되었습니다.  데탑이 독이 되었죠.

게다가 데탑에 우분투까지 설치하였는데.. 영 활용이 되지 않았고 데탑의 XP만을 거의 하루종일 사용하게 되었습니다.

그래서 본래의 연구(?)에 치중하고 간간히 우분투도 활용하는 작업환경을 조성하기 위해 고민한 결과<a href="http://paperinz.com/1289" target="_blank">
paperinz님의 포스트</a>를 발견하게 되었죠. 저런 프로그램이 있다니.. 그래서 여기저기 살핀 결과. 몇 가지 유용한 포스트들을 발견하였습니다.

<a href="http://code.google.com/p/synergy-plus/">http://code.google.com/p/synergy-plus/</a>(개발자 페이지, 다운로드)<a href="http://blog.daum.net/hopark/11953230">
http://blog.daum.net/hopark/11953230</a> (맥용 설치 설명)<a href="http://supaflow.tistory.com/87">
http://supaflow.tistory.com/87</a> (리눅용 설치 설명, 제 설치법과는 많이 다릅니다.)

[caption id="" align="alignnone" width="384" caption="synergy 실행창"]<a title="Flickr에서 siku_kr님의 1" href="http://www.flickr.com/photos/siku_/4031996514/"><img title="synergy 실행창" src="http://farm4.static.flickr.com/3517/4031996514_fdc4acb381.jpg" alt="1" width="384" height="294" /></a>[/caption]

[caption id="" align="alignnone" width="400" caption="synergy 실행창"]<a title="Flickr에서 siku_kr님의 2" href="http://www.flickr.com/photos/siku_/4031996564/"><img title="synergy 실행창" src="http://farm3.static.flickr.com/2669/4031996564_0f366604ca.jpg" alt="2" width="400" height="279" /></a>[/caption]

설치과정은 아주 간단합니다. 먼저 윈도우에서 설명하자면 (1.3.4 버전)
서버에서 설치할 컴퓨터에서

Share this computer’s keyboard and mouse(sever)을 클릭하고

Configure을 클릭&gt; Screens에서 서버와 클라이언트의 컴퓨터 이름을 추가해줍니다. 컴퓨터 이름(내컴퓨터&gt;속성)과 스크린 이름이 틀리다면 따로 설정을 해야됩니다. 이런 과정을 건너뛰기 위해서 스크린 이름은 컴퓨터 이름으로 설정하였습니다.

다음으로 링크를 설정해주어야 하는데 링크는 컴퓨터간의 마우스 위치를 의미합니다. 여기서 주의할 것이 <strong>A 컴의 오른쪽에 B있다</strong>라고 설정하면 반대로 <strong>B컴 왼쪽에 A컴이 있다</strong>라고 추가적으로 설정을 해주어야 합니다.
한 쪽만 설정하면 마우스 커서가 하나의 모니터에 갇히게 된다고 합니다.

<span style="color: #0000ff;"><strong>클라이언트는 어떻게 설정하는지.</strong></span>
클라이언트는 아주 간단합니다. 프로그램을 실행하고 서버컴퓨터의 이름을 적어주면 됩니다.

여기서 주의할 것이(어디에 명시된 것은 아닙니다.)  작업그룹이 서로 같아야 합니다. 저는 WORKGROUP으로 통일했습니다.
우분투에서도 설정을 했는데. 이도 역시 아주 간단합니다.
커맨드 창에서

synergyc –f (서버컴 이름 혹은 아이피) 를 입력하면됩니다.
synergyc –f 111.111.111.11 이런식이죠. (이름으로 하면 잘되지 않는데 해결방법을 잘모르겠네요. samba도 깔고 그렇게 했는데..)

그 결과 제 작업환경이 아래와 같이 바꼈습니다.  왼쪽의 모니터 2대가 노트북, 오른쪽이 데탑이죠.  차이가 확연히 보이죠. (위 설치전, 아래 설치후)
<a title="Flickr에서 siku_kr님의 DSCN3507" href="http://www.flickr.com/photos/siku_/4031208187/"><img src="http://farm4.static.flickr.com/3491/4031208187_70a0b9c0c8.jpg" alt="DSCN3507" width="500" height="163" /></a>

큰 모니터 뒤의 후배자리가 보이는데. 그 후매한테 은폐한 상태로 많은 좋은 것들을 봐왔죠.

<a title="Flickr에서 siku_kr님의 DSCN3508" href="http://www.flickr.com/photos/siku_/4031974128/"><img src="http://farm3.static.flickr.com/2798/4031974128_978276ab1e.jpg" alt="DSCN3508" width="500" height="163" /></a>

(오른쪽은 비스타, 왼쪽은 우분투입니다.)

이거 보신분들 유용히 쓰세요

*  우분투에서 호스트로는 실험하지 않았습니다.
* 데탑의 이름은 우분투나 XP나 모두 동일한 컴퓨터 이름을 사용하였는데 다른 설정을 테스트하지는 않았습니다. 왠지 오류가 나고 시간이 많이 걸릴 것 같아서…
* 한글이 되지 않는 이유는 클라이언트 쪽의 문제라는데... 비스타-xp에서는 기존의 한글패치 없이도 잘되지만 비스타(호스트)-우분투(클라이언트)에서는 이쪽으로 작업한 분들이 없으신 것 같습니다. nabi에서 shift+space는 잘 적용이 안되고 shift+alt를 추가하니까 되기는 하더군요.

