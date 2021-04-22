---
title: "Modern PHP"
categories: PHP
---

> **Modern**
> 1. 현대의, 근대의 (=contemporary)
> 2. 현대적인, 모던한 (=contemporary)
> 3. 최신의 (=up-to-date)   

### Modern PHP
 PHP는 `1995년` 라무스 러도프가 처음 만든 서버사이드 스크립트언어이다.   
 25년 이상 이어진 개발언어로 그동안 많은 변화를 거쳐 현재까지 많은 사람들이 사용하고 있다.   
 그 변화에 맞춰 PHP를 사용하는게 Modern PHP가 아닐까 싶다.
 그렇다면 무조건 최신버전의 PHP를 사용한다고 해서 Modern PHP일까?

 특정한 방법이나 규칙이 있는건 아니다. 하지만 많은 PHP개발자들이 공통적으로 얘기하는 몇가지를 살펴볼까 한다.

**1. 최신버전의 PHP**   
**2. PSR(표준권고) 준수**   
**3. Composer**   


### 1. 최신버전의 PHP
 현재 날짜(2021-04-16) 기준으로 가장 최신 버전의 PHP는 8.0.3(2021-03-04)이다.   
 PHP7버전에서도 그랬듯이 8버전또한 많은 부분이 업데이트 되었다.   
 [PHP공식사이트][phplink]{: target="_blank"}{:: .link} 에서 확인할 수 있다.

### 2. PSR
 개발자 마다 코딩 스타일이 다르다. 수많은 라이브러리와 프레임워크, 컴포넌트들이 있다.    
 표준화가 없다 보니 개발자들은 자신만의 스타일로 코딩을 하고 각각 프레임워크나 라이브러리들의 사용법이나 설치 방법이 달랐고
 이를 해결하기 위해 Laravel, Symfony, CakePHP, Composer 등을 만든 PHP개발자 들이 
 모여 만든 [PHP-FIG(PHP Framework Interoperability Group)][PHP-FIG]{: target="_blank"}{:: .link}에서 
 이에대한 `PHP 표준 권고안(PHP Standards Recommendations)`를 제정하였고 수많은 프레임워크에서 사용하였다.
 

 PSR은 
 1. PHP 커뮤니티 그룹(PHP-FIG) 에서 제정한 PHP 표준 권고안이다.
 2. 권고안이므로 강제성은 없다.
 3. 투표로 표준 권고안이 제정된다.

 통과된 PSR은 전체적으로 읽어보는게 좋다.   
 그 중 많이 접할 수 있는 표준 권고안들은 `PSR-1`, `PSR-4`, `PSR-7`, `PSR-12` 등이 있다.
 
 `PSR-1` - Basic Coding Standard   
 `PSR-4` - Autoloading Standard   
 `PSR-7` - HTTP Message Interface   
 `PSR-12` - Extended Coding Style Guide   

 강제성은 없으므로 필수는 아니지만, Morder PHP 를 지양한다면 필수라고 생각하고 적용해야 할 것 같다.

### 3. Composer

 컴포저는 패키지 관리도구라고 하지 않고 의존성 관리도구라고 한다.   
 필요한 라이브러리들을 선언하고 의존성을 해결해주고 설치 관리해준다.   

- 라이브러리 관리
  컴포저는 라이브러리를 설치 및 업그레이드, 다운그레이드 를 지원한다.
  새로운 라이브러리에 버그나 문제가 있을 경우 새로 설치할 필요없이 다운그레이드로 해결할 수 있다.

- 의존성 지옥 해결

- 라이브러리를 위한 오토로드

<br/><br/><br/><br/><br/><br/>
---
>#### 참고   
>[Modern PHP란? - 권윤학님 블로그][Refernce_1]{: target="_blank"}{:: .link}    
>[Modern PHP & PSR - 이상학님 블로그][Refernce_2]{: target="_blank"}{:: .link}        
>[PHP The Right Way - modernpug.github.io][Refernce_3]{: target="_blank"}{:: .link}     
>[컴포저(Composer) - laravel5 프로그래밍][Refernce_4]{: target="_blank"}{:: .link}   



[phplink]: https://www.php.net/releases/8.0/en.php "Go PHP8.0"
[PHP-FIG]: https://www.php-fig.org/psr "Go PHP-FIG"

[Refernce_1]: https://web-front-end.tistory.com/75 "Modern PHP란?"
[Refernce_2]: https://sanghaklee.tistory.com/44 "Modern PHP & PSR"
[Refernce_3]: http://modernpug.github.io/php-the-right-way/#translations "modernpug.github.io"
[Refernce_4]: https://www.lesstif.com/laravelprog/%EC%BB%B4%ED%8F%AC%EC%A0%80%EC%9D%98-%ED%95%B4%EA%B2%B0%EC%B1%85-26083788.html "laravel5 프로그래밍"
