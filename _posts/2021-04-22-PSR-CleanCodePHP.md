---
title: "PSR 과 Clean Code PHP"
categories: PHP
toc: true
toc_icon: "list"
---

# PSR 과 Clean Code PHP

## 1. PSR

 PSR(PHP Standards Recommendations) 은 PHP 표준 권고안 이다. 
 PSR에 대한 내용은 아래에서 확인할 수 있다.

 >[공식(영문) PHP-FIG(PHP Framework Interoperability Group)][PHP_PSR]{: target="_blank"}{:: .link}   
 >[한글판 PHP Standards Recommendations][PHP_PSR(KR)]{: target="_blank"}{:: .link}   
 *한글번역은 페이스북 'Modern PHP User Group'그룹 관리자분중 한분이신  '김종운'님 gitbook 페이지 이다.

보통 `laravel`, `Symfony`등의 프레임워크를 사용한다면 프레임워크내에 적용되어있어 크게 신경써야할 부분은 없는 것 같다. (때에 따라 사용해야 할 경우도 있다.)
여기서는 `PSR-1`, `PSR-12`에 대해 알아볼까 한다.



### PSR-1, PSR-12

<figure style="max-width: 500px" class="align-center">
   <img src="{{ site.url }}{{ site.baseurl }}/assets/images/coding_style_3.png" alt="">
   <figcaption>F**k Scientology - pinterest</figcaption>
 </figure>       
   
 예전 PSR에 대해 잘 모르거나 적용하지 않았을 때에는 개발자들끼리 들여쓰기, 띄어쓰기, 괄호위치등의 코딩 스타일에 대한 문제로 갈등이 있던 상황을
 심심치 않게 볼 수 있었다. 

#### 다양한 코딩 스타일
   
__[괄호 위치]__

- __GNU__ - 블록을 if문 아래에 작성한다. 이때 중괄호 시작은 들여쓰기로 시작한다.  
 ```php
    if(...)
       {
           처리();
       }
 ```
- __K&R__ - if문과 블록이 같은 라인에 위치한다.
 ```php
    if(...) {
        처리();
    }
 ```
- __BSD__ - 블록을 if문 아래 작성한다. 중괄호 시작은 들여쓰기로 시작하지 않는다.
 ```php
    if(...) 
    {
        처리();
    }
 ```

__[변수/함수 명칭]__

- __카멜 표기법(Camel Case, camelCase) - 여러 단어를 연달아 사용할 때 각 단어의 첫글자를 대문자로 적되, 맨 앞에 오는 글자는 소문자로 표기한다.
```php
    function camelCase(){
        $camelCase = null;
    } 
```
- __파스칼 표기법(Pascal Case, PascalCase) - 이 역시 연달아 오는 단어의 모든 앞글자를 대문자로 표기하는 것은 카멜 표기법과 같지만 맨 앞에 오는 문자를 대문자로 표기한다.
```php
    function PascalCase(){
        $PascalCase = null;
    } 
```
- __스네이크 표기법(Snake Case, snake_case) - 단어 사이에 언더바를 넣어서 표기하는 것이다.
```php
    function snake_case(){
        $snake_case = null;
    } 
```

이와 같이 많은 코딩 스타일들이 존재한다.   
각자 다른 코딩 스타일을 고수한다면 다른사람들과 협업에서 혼란이 가중될 수 있고, 유지보수 측면에서도 어려움이 생길 수 있다.   
이때문에 협업을 하게 될 경우 서로 혼선이 없게 표준안을 정의해놓고 시작하는 경우가 많다.   

__PHP-FIG__ 에서는 PSR을 통해 코딩 스타일 표준안을 재정해 놓았다. `PSR-1`, `PSR-12`가 이에 해당한다.

#### __PSR-1__ - Basic Coding Standard   
>[PSR-1 (공식_영문 PHP Standards Recommendations)][PHP_PSR-1]{: target="_blank"}{:: .link}   
>[PSR-1 (한글판 PHP Standards Recommendations)][PHP_PSR-1(KR)]{: target="_blank"}{:: .link}   

#### __PSR-12__ - Extended Coding Style Guide   
>[PSR-12 (공식_영문 PHP Standards Recommendations)][PHP_PSR-12]{: target="_blank"}{:: .link}   
>[PSR-12 (한글판 PHP Standards Recommendations)][PHP_PSR-12(KR)]{: target="_blank"}{:: .link}   


## 2. Clean Code PHP

개발을 하다보면 혹은 개발을 다 하고나서 자신의 코드를 돌아볼때 내가 짠 코드가 정말 지져분해보이고 이게 맞는 코드인지 확신이 안들 때가 많다.
물론 최선을 다해 코딩을 하지만 그런 생각이 드는건 어쩔 수 없다. 예쁘게 올바르게 효율적으로 코딩하고싶다. 그때 보면 도움이 많이 될 것 같다.   

>__해당 문서 내용 중__   
>Robert C. Martin의 책, 소프트웨어 엔지니어링의 교과서라고 불리는 `Clean Code` PHP 버전입니다. 이 문서는 스타일 가이드가 아닙니다. PHP로 읽기 쉽고 재사용 가능하며, 리팩토링이 쉬운 소프트웨어를 만들어내기 위한 안내서입니다.

#### __Clean Code PHP__ 
>[Clean Code PHP (공식_영문 Clean Code PHP)][Clean Code PHP]{: target="_blank"}{:: .link}   
>[Clean Code PHP (한글판 Clean Code PHP)][Clean Code PHP(KR)]{: target="_blank"}{:: .link}


## 마치며
 항상 이렇게 영문화 된 내용을 번역해주시는 분들께 감사하는 마음을 가지고 개발을 하고 있습니다.

<br/><br/><br/><br/><br/><br/>
---
>#### 참고   
>[공식(영문) PHP-FIG(PHP Framework Interoperability Group)][PHP_PSR]{: target="_blank"}{:: .link}   
>[한글판 PHP Standards Recommendations][PHP_PSR(KR)]{: target="_blank"}{:: .link}      
>[F&#42;&#42;k Scientology - pinterest][F**kScientology]{: target="_blank"}{:: .link}   
>[코딩스타일 - 나무위키][namu.wiki]{: target="_blank"}{:: .link}

[PHP_PSR]: https://www.php-fig.org/psr "PHP-FIG"
[PHP_PSR-1]: https://www.php-fig.org/psr/psr-1/ "PHP-FIG"
[PHP_PSR-12]: https://www.php-fig.org/psr/psr-1/ "PHP-FIG"
[PHP_PSR(KR)]: https://www.php-fig.org/psr "한글판 PHP PSR"
[PHP_PSR-1(KR)]: https://psr.kkame.net/accepted/psr-1-basic-coding-standard "한글판 PHP PSR-1"
[PHP_PSR-12(KR)]: https://psr.kkame.net/accepted/psr-12-extended-coding-style-guide "한글판 PHP PSR-12"
[namu.wiki]: https://namu.wiki/w/%EC%BD%94%EB%94%A9%20%EC%8A%A4%ED%83%80%EC%9D%BC "나무위키"
[F**kScientology]: https://www.pinterest.co.kr/pin/390898442655218803/ "pinterest"

[Clean Code PHP]: https://github.com/jupeter/clean-code-php "Clean Code PHP"
[Clean Code PHP(KR)]: https://github.com/yujineeee/clean-code-php "Clean Code PHP(KR)"
