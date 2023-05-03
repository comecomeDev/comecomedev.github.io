---
title: Package Manager
author: 05-02 23:10:00 +0800
categories: [Study, Node]
tags: [Network]
render_with_liquid: false
---



## Package Manager

 + 패키지 매니저는 패키지를 손쉽게 다둘수 있는 툴로 대표적인 패키지 매니저는 yarn과 npm이 있음 
    여기서 말하는 패키지는 yarn 또는 npm에 업로드된 Node.js모듈을 패키지라고 함 
    모듈이 다른모듈을 참조하여 의존관계를 가질수 있음
    npm(Node Package Manager) node.js와 관계없이 프론트 단에서만 사용가능한 패키지도 등록되어 있음
    yarn 은 FaceBook이 출시한 패키지 매니저로 npm보다 빠른 속도로 관리가능 (아래 url를 참조 =>
    <https://soshace.com/yarn-package-manager-in-2019-should-we-keep-on-comparing-yarn-with-npm/> )    npm과 yarn은 동시에 사용할경우 각 설치한 버전이 다르게 관리될수 있어 충돌할 가능성이 크다 그렇게 때문에 한가지 패키지관리자를 사용하는게 좋음

    Package.json : 설치한 패키지에 버전관리 및 프로젝트명,작성자,라이센스 정보 등 메타데이터를 기록가능한 파일 
    여기서 메타데이터는 데이터를위한데이터라는 표현으로 어떤 목적을가진 데이터라고 표현되기도 하며 
    Package-lock.json : Package.json파일에서 정의한 파일이외에도 node_modules에 들어있는 패키지들의 버전과 의존관계가 상세히 기록되며 npm으로 패키지를 설치,수정,삭제될때마다 패키지의 의존관계를 저장함



    -npm init 명령어를 통해 pacakage.json 를 설치가능


