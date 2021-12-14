# To Become a Better Programmer
## 설명
Description에도 써있다시피 jwasham의 Coding Interview University에서 영감을 받아 시작하게 되었다.
물론 해당 저장소에도 [한국어로 번역된 판](https://github.com/jwasham/coding-interview-university/blob/master/translations/README-ko.md)이 존재하지만
막상 뚜껑을 열어보면 안내만 한글일 뿐이지 그가 걸어놓은 링크나 자료 모두 영어로 구성돼있단 걸 알 수 있을 것이다.
물론 영어에 능숙하면 그가 올려놓은 양질의 자료를 쉽고 빠르게 탐독할 수 있겠지만 나는 영어에 능숙하지 않은 프로그래머들이 한국에 많이 있다는 걸 안다.
나 또한 그 중 하나이다. 

그런 의미로 여기에서 한국판 Coding Interview University를 작성하려 한다.
약간의 차이가 있다면 Interview University라는 이름과는 달리 코딩 면접을 위한 프로젝트는 아니라는 점이다.
그냥 스스로도 더 나은 프로그래머가 되고 싶어서, 또 한글로 된 양질의 자료도 많은데 파편화돼있는 게 아쉬워서 시작하게 됐다.
그래서 저장소의 이름 자체도 To Become a Better Programmer(더 나은 프로그래머 되기)로 정하였다.


되도록이면 한글로 된 자료 중에 쉽고 알아보기 쉬운 자료를 차용할 것이며, 직접 코드를 써야할 경우에는
비전공자들도 쉽게 알아볼 수 있는 python3으로 작성할 예정이다.
목차나 내용은 jwasham의 Coding Interview University을 참고할 것이나 완전히 같지는 않을 것이며, 정렬은 123->abc->가나다 순서대로 할 것이다.
그리고 [내 블로그](https://this-programmer.tistory.com/)에 있는 글들도 이용할 예정이다.

## 목차
- [네트워크(Network)](#네트워크)
- [데이터베이스(Database)](#데이터베이스)
- [디자인패턴(Design Pattern)](#디자인패턴)
- [생산성 향상 도구들(Utilities)](#생산성-향상-도구들)
- [소프트웨어 공학(Software engineering)](#소프트웨어-공학)
- [소프트웨어 인프라(Software infrastructure)](#소프트웨어-인프라)
- [알고리즘(Algorithm)](#알고리즘)
- [인공지능(Artificial Intelligence)](#인공지능)
- [언어(Language)](#언어)
- [운영체제(Operating System)](#운영체제)
- [자료구조(Data Structure)](#자료구조)
- [좋은 글들(Wellmade Posts)](#좋은-글들)
- [컴퓨터 공학(Computer engineering)](#컴퓨터-공학)  

## 네트워크
- [GET과 POST의 차이](https://hongsii.github.io/2017/08/02/what-is-the-difference-get-and-post/)
- [HTTP와 HTTPS의 차이점](https://dany-it.tistory.com/96)
- [HTTP Protocols](https://ko.wikipedia.org/wiki/HTTP)
- [JSON이란?](https://ko.wikipedia.org/wiki/JSON)
- [OAuth란? 그리고 OAuth1, OAuth2](https://minwan1.github.io/2018/02/24/2018-02-24-OAuth/)
- [OAuth2를 이용한 SSO 환경 구축 (1/2)](http://www.nextree.co.kr/oauth-2reul-iyonghan-sso-hwangyeong-gucug-1-2/)
- [OAuth2를 이용한 SSO 환경 구축 (2/2)](http://www.nextree.co.kr/oauth-2reul-iyonghan-sso-hwangyeong-gucug-2-2/)
- RestAPI
    - [REST API 제대로 알고 사용하기](https://meetup.toast.com/posts/92)
    - [그놈의 RESTful API. 한 줄로 정의하자면](https://this-programmer.tistory.com/entry/%EA%B7%B8%EB%86%88%EC%9D%98-RESTful-API-%ED%95%9C-%EC%A4%84%EB%A1%9C-%EC%A0%95%EC%9D%98%ED%95%98%EC%9E%90%EB%A9%B4)
- [SSO(Single Sign-On)이란?](https://toma0912.tistory.com/75)
- [TCP/IP의 이해](https://m.blog.naver.com/jhc9639/221411218450?referrerCode=1)
- 로드밸런싱(Load Balancing)
    - [로드 밸런서(Load Balancer)란?](https://nesoy.github.io/articles/2018-06/Load-Balancer)
    - [로드밸런싱방식 종류](https://medium.com/@pakss328/%EB%A1%9C%EB%93%9C%EB%B0%B8%EB%9F%B0%EC%84%9C%EB%9E%80-l4-l7-501fd904cf05)
- [브라우저의 렌더링 과정](https://medium.com/%EA%B0%9C%EB%B0%9C%EC%9E%90%EC%9D%98%ED%92%88%EA%B2%A9/%EB%B8%8C%EB%9D%BC%EC%9A%B0%EC%A0%80%EC%9D%98-%EB%A0%8C%EB%8D%94%EB%A7%81-%EA%B3%BC%EC%A0%95-5c01c4158ce)
- [웹 브라우저에 URL을 입력하면 어떤 일이 일어날까?](https://owlgwang.tistory.com/1)
- [웹의 동작 원리](https://velog.io/@wonhee010/%EC%9B%B9%EC%9D%98-%EB%8F%99%EC%9E%91-%EC%9B%90%EB%A6%AC)
- [쿠키와 세션의 차이](https://jeong-pro.tistory.com/80)
- 프록시 서버(Proxy Server)
    - [프록시 서버란?(1)](https://brownbears.tistory.com/191)
    - [프록시 서버란?(2)](https://soul0.tistory.com/230)
    
## 데이터베이스
- [Clustering vs Replication vs Sharding](https://jordy-torvalds.tistory.com/94)
- [Lock에 대해서 알아보자 - 기본편](https://sabarada.tistory.com/121)
- [MongoDB의 Transaction과 session문제](https://crmrelease.tistory.com/138)
- [ORM이란](https://gmlwjd9405.github.io/2019/02/01/orm.html)
- [데이터베이스 튜닝 (DB Tuning)](http://blog.skby.net/%EB%8D%B0%EC%9D%B4%ED%84%B0%EB%B2%A0%EC%9D%B4%EC%8A%A4-%ED%8A%9C%EB%8B%9D-db-tuning/)
- [왜 데이터베이스(DB) 튜닝을 해야할까?](https://travislife.tistory.com/25)
- [인덱스(index)란?](https://mangkyu.tistory.com/96)
- [저장 프로시저](https://ko.wikipedia.org/wiki/%EC%A0%80%EC%9E%A5_%ED%94%84%EB%A1%9C%EC%8B%9C%EC%A0%80)
- [정규화(Normalization)](https://mangkyu.tistory.com/28?category=761304)
- [클러스터링 vs 리플리케이션 vs 샤딩](https://velog.io/@gkskaks1004/%ED%81%B4%EB%9F%AC%EC%8A%A4%ED%84%B0%EB%A7%81-vs-%EB%A6%AC%ED%94%8C%EB%A6%AC%EC%BC%80%EC%9D%B4%EC%85%98-vs-%EC%83%A4%EB%94%A9)
- [트랜잭션 격리 수준(Transaction Isolation Level)](https://dar0m.tistory.com/225)
- [트랜잭션이란? (Transaction)](https://limkydev.tistory.com/100?category=974039)
- [트랜잭션과 격리성](https://sabarada.tistory.com/117)
- [트랜잭션(transaction)이란?(1)](https://mommoo.tistory.com/62)
- [트랜잭션(transaction)이란?(2)](https://devuna.tistory.com/30)
- [트리거(Trigger)란?](https://limkydev.tistory.com/154)
- [효과적인 DB index 설정하기](https://velog.io/@jwpark06/%ED%9A%A8%EA%B3%BC%EC%A0%81%EC%9D%B8-DB-index-%EC%84%A4%EC%A0%95%ED%95%98%EA%B8%B0)

## 디자인패턴
- [Design Patterns on python](https://brownbears.tistory.com/category/%EA%B3%B5%EB%B6%80/%EB%94%94%EC%9E%90%EC%9D%B8%20%ED%8C%A8%ED%84%B4)
- [MVC패턴이란](https://m.blog.naver.com/jhc9639/220967034588)
    
## 생산성 향상 도구들
- [ERD CLOUD](https://www.erdcloud.com/)
- [gitstar-ranking(깃허브 별 개수 랭킹 알려주는 사이트)](https://gitstar-ranking.com)
- [Graphviz 소개](https://narusas.github.io/2019/01/25/Graphviz.html)
- [POSTMAN과 JSON Placeholder(JSON을 테스트하는 가장 좋은 방법)](https://this-programmer.tistory.com/entry/JSON%EC%9D%84-%ED%85%8C%EC%8A%A4%ED%8A%B8%ED%95%98%EB%8A%94-%EA%B0%80%EC%9E%A5-%EC%A2%8B%EC%9D%80-%EB%B0%A9%EB%B2%95-POSTMAN%EA%B3%BC-JSON-Placeholder?category=767889)
- [regex101.com(정규식 짤 때 도움되는 사이트)](https://this-programmer.tistory.com/entry/%EC%A0%95%EA%B7%9C%EC%8B%9D-%EC%A7%A4-%EB%95%8C-%EC%97%84%EC%B2%AD%EB%82%98%EA%B2%8C-%EB%8F%84%EC%9B%80%EC%9D%B4-%EB%90%98%EB%8A%94-%EC%82%AC%EC%9D%B4%ED%8A%B8-regex101com?category=772368)
- [[Telegraf + influxDB + Grafana]10분만에 데브옵스를 위한 모니터링 시스템 구축하기](https://blog.voidmainvoid.net/91])
- [Wappalyzer(웹사이트 구성요소를 볼 수 있는 크롬 확장 프로그램)](https://this-programmer.tistory.com/entry/%EC%9B%B9%EC%82%AC%EC%9D%B4%ED%8A%B8%EB%A5%BC-%EB%AD%98%EB%A1%9C-%EB%A7%8C%EB%93%A4%EC%97%88%EB%8A%94%EC%A7%80-%EC%95%8C-%EC%88%98-%EC%9E%88%EA%B2%8C-%ED%95%B4%EC%A3%BC%EB%8A%94-%ED%81%AC%EB%A1%AC-%ED%99%95%EC%9E%A5-%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%A8-Wappalyzer?category=772368)
- [무료 DB Tool (DBeaver)](https://m.blog.naver.com/skykbc/221426494422)
- 깃(Git)
    - [Git Rebase & Squash](https://velog.io/@ppl8709/git-rebase)
    - [Github에 잘못 올라간 파일 삭제하기](https://gmlwjd9405.github.io/2018/05/17/git-delete-incorrect-files.html)
    - [초심자를 위한 Github 협업 튜토리얼 (with 토끼와 거북이)](https://milooy.wordpress.com/2017/06/21/working-together-with-github-tutorial/)
- 도커(Docker)
    - [도커 컨테이너는 가상머신인가요? 프로세스인가요?](https://www.44bits.io/ko/post/is-docker-container-a-virtual-machine-or-a-process)
    - [도커(Docker)로 CentOS 이미지 systemctl 사용하기](https://this-programmer.tistory.com/entry/%EB%8F%84%EC%BB%A4Docker%EB%A1%9C-CentOS-%EC%9D%B4%EB%AF%B8%EC%A7%80-systemctl-%EC%82%AC%EC%9A%A9%ED%95%98%EA%B8%B0-2-failed-to-get-DBus-connection-Operation-not-permitted)
    - [초보를 위한 도커 안내서 - 도커란 무엇인가?](https://subicura.com/2017/01/19/docker-guide-for-beginners-1.html)
- 쿠버네티스(Kubernetes, k8s)
    - [쿠버네티스 Ingress 개념 및 적용방법](https://twofootdog.tistory.com/23)
    
## 소프트웨어 공학
- [Call by Value와 Call by Reference](https://re-build.tistory.com/3)
- [장애 허용 시스템](https://ko.wikipedia.org/wiki/%EC%9E%A5%EC%95%A0_%ED%97%88%EC%9A%A9_%EC%8B%9C%EC%8A%A4%ED%85%9C)
- [프로그램과 프로세스와 스레드의 차이](https://velog.io/@raejoonee/%ED%94%84%EB%A1%9C%EC%84%B8%EC%8A%A4%EC%99%80-%EC%8A%A4%EB%A0%88%EB%93%9C%EC%9D%98-%EC%B0%A8%EC%9D%B4)
- [프로세스 격리란 무엇입니까?](https://www.netinbag.com/ko/internet/what-is-process-isolation.html)
- [함수(function)와 메소드(method)의 차이](https://this-programmer.tistory.com/entry/%ED%95%A8%EC%88%98Function%EC%99%80-%EB%A9%94%EC%86%8C%EB%93%9CMethod%EC%9D%98-%EC%B0%A8%EC%9D%B4)

## 소프트웨어 인프라
- [devops란 - from aws](https://aws.amazon.com/ko/devops/what-is-devops/)
- [Failover, 페일오버란 무엇인가](https://m.blog.naver.com/on21life/221221178100)
- [데이터 파이프라인이란 무엇인가?](https://blog.voidmainvoid.net/265)
- [배포 방법 정리 (고정/롤링/블루-그린/카나리 릴리즈 배포)](https://devpouch.tistory.com/136)
- [오케스트레이션(Orchestration)이란?](https://www.redhat.com/ko/topics/automation/what-is-orchestration)
- [코드형 인프라(IaC)란?](https://www.redhat.com/ko/topics/automation/what-is-infrastructure-as-code-iac)
- [프로비저닝(Provisioning)이란? 개념, 종류, 자동화 방법](https://www.redhat.com/ko/topics/automation/what-is-provisioning)
- [현기증나는 인프라, 배포 용어들(IaC, 오케스트레이션, CI/CD, DEVOPS, 프로비저닝 등등) 정리](https://this-programmer.tistory.com/447)

## 알고리즘
- [DFS와 BFS](https://this-programmer.tistory.com/entry/%EB%B0%B1%EC%A4%801260%ED%8C%8C%EC%9D%B4%EC%8D%AC-DFS%EC%99%80-BFS)
- [FizzBuzz 문제](https://bryan.wiki/260)
- [Lock Free 알고리즘(Non-Blocking 알고리즘)](https://effectivesquid.tistory.com/entry/Lock-Free-%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98Non-Blocking-%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98)
- [논 블로킹 알고리즘(Non-blocking Algorithms)](https://parkcheolu.tistory.com/33)
- [동적 계획법(Dynamic Programming)](https://ko.wikipedia.org/wiki/%EB%8F%99%EC%A0%81_%EA%B3%84%ED%9A%8D%EB%B2%95)
- [브루트 포스(Brute Force)](https://steemit.com/kr-dev/@gyeryak/easyalgo-2-bruteforce)
- [빅오 표기법(Big-O Notation), 시간 복잡도, 공간 복잡도](https://cjh5414.github.io/big-o-notation/)
- [에라토스테네스의 체(Sieve of Eratosthenes)](https://ko.wikipedia.org/wiki/%EC%97%90%EB%9D%BC%ED%86%A0%EC%8A%A4%ED%85%8C%EB%84%A4%EC%8A%A4%EC%9D%98_%EC%B2%B4)
- [이진탐색](https://namu.wiki/w/%EC%9D%B4%EC%A7%84%20%ED%83%90%EC%83%89)
- [정렬 알고리즘](https://namu.wiki/w/%EC%A0%95%EB%A0%AC%20%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98)
- [정렬 알고리즘 비교](https://ratsgo.github.io/data%20structure&algorithm/2017/10/19/sort/)
- [탐욕법(Greedy Algorithm)과 그 종류](https://janghw.tistory.com/entry/%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98-Greedy-Algorithm-%ED%83%90%EC%9A%95-%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98)
- [피보나치 수열을 구하는 세 가지 방법. (재귀, 동적 계획법, 반복)](https://makefortune2.tistory.com/60)
- [해시 함수](https://ko.wikipedia.org/wiki/%ED%95%B4%EC%8B%9C_%ED%95%A8%EC%88%98)

## 자료구조
- [B-Tree, B+ Tree](https://ssup2.github.io/theory_analysis/B_Tree_B+_Tree/)
- [Rope](https://en.wikipedia.org/wiki/Rope_(data_structure))
- [Linked list (연결 리스트) 란 무엇인가?](https://supermemi.tistory.com/67)
- [배열(Array)과 리스트(List)](https://wayhome25.github.io/cs/2017/04/17/cs-18-1/)
- [이진 트리(Binary Tree)의 종류](https://hsc-tech.tistory.com/7)
- [이진 트리](https://thebook.io/007031/part01/ch03/07/01/)
- [이진탐색트리(Binary Search Tree)](https://ratsgo.github.io/data%20structure&algorithm/2017/10/22/bst/)
- [자료구조와 시간복잡도](https://daelumgi.postype.com/post/5270208)
- [해시맵 (HashMap) / 맵 (Map)](https://hapbbying.tistory.com/81)
- [효율적인 긴 문자열 연산을 위한 Rope 자료구조](http://www.secmem.org/blog/2019/03/09/rope/)
- [힙(heap)이란](https://gmlwjd9405.github.io/2018/05/10/data-structure-heap.html)

## 언어
- 자바(Java)
    - [코드로 알아보는 java의 Hashmap](https://sabarada.tistory.com/57)
- 자바스크립트(Javascript)
    - [자바스크립트의 변수범위와 호이스팅](http://chanlee.github.io/2013/12/10/javascript-variable-scope-and-hoisting/)
- 파이썬(Python)
    - [[Python] 튜플(tuple), 리스트(list), 셋(set), 딕셔너리(dict) 비교](https://specialscene.tistory.com/142#:~:text=%EB%A6%AC%EC%8A%A4%ED%8A%B8%EC%99%80%20%EB%B9%84%EA%B5%90%EA%B0%80%20%EB%A7%8E%EC%9D%B4,%ED%95%98%EA%B1%B0%EB%82%98%20%EB%B3%80%EA%B2%BD%ED%95%A0%20%EC%88%98%20%EC%97%86%EB%8B%A4%EB%8A%94%20%EA%B2%83.)
    - [데코레이터(decorator)란?](https://hello-bryan.tistory.com/214)
    - [제네레이터(generator)란?(1)](https://bluese05.tistory.com/56)
    - [제네레이터(generator)란?(2)](https://wikidocs.net/16069)
    - [파이썬의 대표적인 네 자료형(리스트, 셋, 튜플, 딕셔너리) 특성 알아보기](https://this-programmer.tistory.com/445)

## 인공지능
- [MLOps 란 무엇일까?](https://medium.com/daria-blog/mlops-%EB%9E%80-%EB%AC%B4%EC%97%87%EC%9D%BC%EA%B9%8C-7ba8d9aae221)
- [딥러닝이란 무엇인가](https://tensorflow.blog/%EC%BC%80%EB%9D%BC%EC%8A%A4-%EB%94%A5%EB%9F%AC%EB%8B%9D/1-%EB%94%A5%EB%9F%AC%EB%8B%9D%EC%9D%B4%EB%9E%80-%EB%AC%B4%EC%97%87%EC%9D%B8%EA%B0%80/)

## 운영체제
- [Deadlock 개념이란? 그에 대한 해결책/회피책](https://jwprogramming.tistory.com/12)
- [데드락(Deadlock, 교착 상태)이란?](https://chanhuiseok.github.io/posts/cs-2/)
- [운영 체제(위키)](https://ko.wikipedia.org/wiki/%EC%9A%B4%EC%98%81_%EC%B2%B4%EC%A0%9C)
- 리눅스(Linux) / 유닉스(Unix)
    - [Linux - Namespace 란?](https://galid1.tistory.com/442)
    - [cgroup 이란?](https://sonseungha.tistory.com/535)
    - [리눅스(Linux)와 유닉스(Unix)의 차이](https://this-programmer.tistory.com/entry/%EB%A6%AC%EB%88%85%EC%8A%A4Linux%EC%99%80-%EC%9C%A0%EB%8B%89%EC%8A%A4Unix%EC%9D%98-%EC%B0%A8%EC%9D%B4)
    - [리눅스 네임스페이스(Linux Namespace)란?](https://www.44bits.io/ko/keyword/linux-namespace)
- 윈도우(Window)

## 좋은 글들
- [CRM이란 무엇인가요?](https://www.oracle.com/kr/cx/what-is-crm/)
- [IT직군에서 많이 쓰이는 SI, SM, SE, PG 등 용어의 의미](https://this-programmer.tistory.com/entry/IT%EC%A7%81%EA%B5%B0%EC%97%90%EC%84%9C-%EB%A7%8E%EC%9D%B4-%EC%93%B0%EC%9D%B4%EB%8A%94-SI-SM-SE-PG-%EB%93%B1-%EC%9A%A9%EC%96%B4%EC%9D%98-%EC%9D%98%EB%AF%B8)
- [OKR이란?](https://experience.dropbox.com/ko-kr/resources/what-is-an-okr)
- [POC (Proof Of Concept)란?](https://m.blog.naver.com/pmw9440/221763425946)
- [네이버 메인 페이지의 트래픽 처리](https://d2.naver.com/helloworld/6070967)
- [소프트웨어, 실무형 인재의 신화](https://sangminpark.blog/2011/08/26/%EC%86%8C%ED%94%84%ED%8A%B8%EC%9B%A8%EC%96%B4-%EC%8B%A4%EB%AC%B4%ED%98%95-%EC%9D%B8%EC%9E%AC%EC%9D%98-%EC%8B%A0%ED%99%94/)
- [통합관제 EMS(종합관제)](http://hamonsoft.co.kr/solution/integrated-control/integrated-management/netis-ems/)

## 컴퓨터 공학
- [10분 Actor Model 정리](https://hyojabal.tistory.com/1)
- [컴퓨터가 1+1을 하는 과정](https://brunch.co.kr/@lqju/8)
- [메모리의 구조 (코드, 데이터, 힙, 스택 영역)](https://all-young.tistory.com/17)
- [행위자 모델](https://ko.wikipedia.org/wiki/%ED%96%89%EC%9C%84%EC%9E%90_%EB%AA%A8%EB%8D%B8)
