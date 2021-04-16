---
title: "Modern PHP"
categories: daily
---

> **Modern**
> 1. 현대의, 근대의 (=contemporary)
> 2. 현대적인, 모던한 (=contemporary)
> 3. 최신의 (=up-to-date)   

### ModernPHP
 PHP는 `1995년` 라무스 러도프가 처음 만든 서버사이드 스크립트언어이다.   
 25년 이상 이어진 개발언어로 그동안 많은 변화를 거쳐 현재까지 많은 사람들이 사용하고 있다.   
 그 변화에 맞춰 PHP를 사용하는게 ModernPHP가 아닐까 싶다.
 그렇다면 무조건 최신버전의 PHP를 사용한다고 해서 ModernPHP일까?

 특정한 방법이나 규칙이 있는건 아니다. 하지만 많은 PHP개발자들이 공통적으로 얘기하는 몇가지를 살펴볼까 한다.

**1. 최신버전의 PHP**   
**2. PSR(표준권고) 준수**   
**3. Composer**   


### 1. 최신버전의 PHP
 현재 날짜(2021-04-16) 기준으로 가장 최신 버전의 PHP는 8.0.3(2021-03-04)이다.   
 PHP7버전에서도 그랬듯이 8버전또한 많은 부분이 업데이트 되었다.   
 [PHP공식사이트][phplink]에서 확인할 수 있다. 자세한 내용은 나중에 따로 다뤄볼까 한다.

### 2. PSR
 개발자 마다 코딩 스타일이 다르다. 수많은 라이브러리와 프레임워크, 컴포넌트들이 있다.    
 개발자들은 각각 자신만의 스타일로 코딩을 하고   
 긴 시간동안 이어진 습관들을 고치기란 쉽지 않다.   
 하지만 혼자 일하는 개발자들은 많지 않고 함께 협업을 하기 위해선
 가능한 공통적인 코드스타일을 적용하는게 중요하다.

 ...

### 3. Composer

 컴포저는 패키지 관리도구라고 하지 않고 의존성 관리도구라고 한다.   
 필요한 라이브러리들을 선언하고 의존성을 해결해주고 설치 관리해준다.   

- 라이브러리 관리
  컴포저는 라이브러리를 설치 및 업그레이드, 다운그레이드 를 지원한다.
  새로운 라이브러리에 버그나 문제가 있을 경우 새로 설치할 필요없이 다운그레이드로 해결할 수 있다.

- 의존성 지옥 해결

- 라이브러리를 위한 오토로드



>#### 참고
>[Modern PHP란? - 권윤학님 블로그][Refernce_1]   
>[Modern PHP & PSR - 이상학님 블로그][Refernce_2]   
>[PHP The Right Way - modernpug.github.io][Refernce_3]
> 
>[컴포저(Composer) - laravel5 프로그래밍][Refernce_4]


[phplink]: https://www.php.net/releases/8.0/en.php "Go google"

[Refernce_1]: https://web-front-end.tistory.com/75 "Modern PHP란?"
[Refernce_2]: https://sanghaklee.tistory.com/44 "Modern PHP & PSR"   

[Refernce_3]: http://modernpug.github.io/php-the-right-way/#translations "modernpug.github.io"

[Refernce_4]: https://www.lesstif.com/laravelprog/%EC%BB%B4%ED%8F%AC%EC%A0%80%EC%9D%98-%ED%95%B4%EA%B2%B0%EC%B1%85-26083788.html "laravel5 프로그래밍"
