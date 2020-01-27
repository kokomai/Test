---
layout: post
title: "Spring Legacy Project의 구조에 대하여"
date: 2020-01-27
background: '/img/posts/test.jpeg'
---

 
# Spring Legacy Project란 무엇인가?

Spring Legacy Project 를 사전적인 의미로 풀면,  
 Spring은 우리가 사용하는 Framework를 의미하겠고  
 Legacy란 유산을 뜻하는데, 스프링에서 사용하는 구조를   
 `유산`으로 상속받는 듯한 느낌을 받는다.  
 
 
 어떻게 보면 이는 맞는말일 수 있다.  
 실제로, Spring framework의 구조에 맞게끔 프로젝트 구조가 만들어지니 말이다.
 
 
 이 Spring Legacy Project (이제부터 줄여서 SLP라고 표현하겠다.)는  
 자체적으로 Maven을 활용하여 사용자가 원하는 다양한 jar 파일들을   
 pom.xml에 <dependency>로 입력하면  
 자동으로 찾아서 다운로드 해준다.
 
 
 이는 다른 업무를 맡고 있는 팀원들과 프로젝트를 합쳤을 때  
 필요한 jar파일이 각각 다른데, 이를 카톡이나 메일로 일일히 옮겨서  
 프로젝트를 병합하는 것 보다는 pom.xml에 구문 하나를 추가하거나 복사하여  
 간편하게 적용할 수 있다는 이점을 갖고 있다.
 
 
 이러한 설명을 듣고 마침 Github를 활용하여 프로젝트 버전관리를 하고    
 개별 업무의 병합을 꾀하던 찰나에 필요한 기능이라 생각하여  
 학원 수료 뒤 기존에 하던 프로젝트를 버전업 하여 재 배포할 때에는  
 STS를 사용하여 Spring Legacy Project를 구축하고 Github를 통해 버전관리를  
 하고자 하였다.
 
 
 그렇게 STS를 설치하였는데, 아니나 다를까 이게 도통 무슨 구조인지 이해가
 가질 않았다.   
 
 남들이 하는 대로, SLP를 만들면 무얼 하나... src는 왜 JavResources에 여러개로  
 분리되어 있는 것이며, Maven은 또 어떻게 의존성 삽입을 하는건지..  
 도대체 어디다가 Java 코딩을 하고, 어디에다가 viewpage를 담당할 jsp를 넣는지..  
 
 
 
 
 
 

