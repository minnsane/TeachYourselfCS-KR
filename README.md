# 컴퓨터과학 스스로 학습하기

원문 : **[Teach Yourself Computer Science](https://teachyourselfcs.com/)**

노트 : 이 가이드는 2020년 5월에 확장 업데이트 되었습니다. 이전 버전은 [여기](https://teachyourselfcs.com/2016/)를 참조해주세요.

만약 당신이 독학 엔지니어나 부트캠프 졸업생이라면, 컴퓨터 과학을 배우는 것도 놓쳐서는 안됩니다.   
다행스럽게도, 시간이나 학위를 위한 학자금 투자 없이 월드클래스 컴퓨터과학(Computer Science, 이하 CS) 교육을 받을 수 있습니다.💸
      
세상엔 수많은 리소스가 있지만, 어떤 것들은 다른 것들보다 더 뛰어납니다. 당신에겐 '200개가 넘는 무료 온라인 코스' 같은 리스트는 필요 없습니다. 다음 질문에 답만 있으면 됩니다:
* **어떤 과목**을 배워야 하며, 왜 배워야 하는가?
* 각 과목 **최고의 책 또는 영상 강의**는 무엇인가?   

이 가이드는 이러한 질문에 확실한 답을 주기 위한 우리의 노력입니다.   

## 요약
아래의 아홉 과목을 대략적으로 나열된 순서대로 추천 도서나 강의를 통해(둘 다 보는게 이상적) 학습하세요.
각 과목당 100-200시간 정도 투자하여 공부하고, 나중에 일할면서 필요할때 다시 찾아보세요.🚀

|과목|왜 공부해야 하는가?|책|영상|
|---|--------------|-|---|
|[프로그래밍](#프로그래밍)|재귀 같은 걸 "완전히 이해하지는 못한" 사람이 되지 마세요.|Structure and Interpretation of Computer Programs|Brian Harvey’s Berkeley CS 61A|
|[컴퓨터구조](#컴퓨터구조)|컴퓨터가 실질적으로 어떻게 작동하는 지에 관한 확실한 멘탈모델이 없다면, 더 높은 단계의 추상화는 다루기 힘들겁니다.|Computer Systems: A Programmer's Perspective|Berkeley CS 61C|
|[알고리즘과 자료구조](#알고리즘과-자료구조)|스택, 큐, 트리나 그래프 같은 항상 보이는 자료구조에 대한 이해가 없다면, 문제 풀이는 할 수 없을 것입니다.|The Algorithm Design Manual|Steven Skiena’s lectures|
|[CS를 위한 수학](#컴퓨터-과학을-위한-수학)|컴퓨터 과학이 본래 응용수학의 탈주 브랜치인만큼, 수학을 배워 경쟁력을 높일 수 있습니다.|Mathematics for Computer Science|Tom Leighton’s MIT 6.042J|
|[운영체제](#운영체제)|당신이 짠 코드 대부분은 운영체제에 의해 실행되니, 어떻게 상호작용하는지 알아야합니다.|Operating Systems: Three Easy Pieces|Berkeley CS 162|
|[컴퓨터 네트워킹](#컴퓨터-네트워킹)|인터넷은 매우 중요해졌습니다. 어떻게 동작하는지 이해하고 그 엄청난 잠재력을 깨워보세요.|Computer Networking: A Top-Down Approach|Stanford CS 144|
|[데이터베이스](#데이터베이스)|데이터베이스는 대부분의 중요한 프로그램의 핵심이지만, 어떻게 동작하는지 제대로 이해하는 사람은 거의 없습니다.|Readings in Database Systems|Joe Hellerstein’s Berkeley CS 186|
|[언어와 컴파일러](#언어와-컴파일러)|언어와 컴파일러가 실제 어떻게 동작하는지 이해한다면, 더 나은 코드를 작성하고 새로운 언어를 쉽게 배울 수 있습니다.|Crafting Interpreters|Alex Aiken’s course on edX|
|[분산시스템](#분산시스템)|요즘은 *대부분*의 시스템이 분산시스템입니다.|Designing Data-Intensive Applications by Martin Kleppmann|MIT 6.824|

## 그래도 너무 많죠?
9개 과목을 몇년동안 자습해야 한다는 사실이 너무 부담스럽다면, 두 가지 책에 집중하기를 추천 드립니다: *Computer Systems: A Programmer's Perspective(번역본: 컴퓨터시스템)* 과 *Designing Data-Intensive Applications(번역본: 데이터 중심 애플리케이션 설계)*. 우리가 경험해 본 바, 이 두 책이 특히 네트워크 어플리케이션 관련된 일을 하는 독학 엔지니어와 부트캠프 졸업생에게 들인 시간 대비 고효율을 제공합니다. 이 책들은 위 리스트의 다른 주제들을 위한 맛보기가 되기도 할 거에요.

## 왜 컴퓨터 과학을 배워야 하는가?
세상에는 두 부류의 소프트웨어 엔지니어가 있습니다: 도전적이고, 혁신적인 일을 할 만큼 컴퓨터 과학을 잘 이해하고 있는 사람들 혹은 몇가지 하이레벨 툴을 익혀 겨우겨우 해나가는 사람들.    
두 부류 모두 자신을 소프트웨어 엔지니어라고 칭하며, 커리어 초기에는 비슷한 연봉을 받곤 합니다. 하지만 해가 거듭되며 전자가 중요한 상업 프로젝트던 엄청난 오픈소스 프로젝트이던 좀 더 성취감있고 보수가 좋은 일을 하며 기술적인 리더쉽을 쌓거나 고퀄리티의 개인적 성취를 이뤄 나갑니다.    
     
첫번째 부류의 엔지니어들은 컴퓨터 과학을 전통적 방법이나 커리어동안 가차없이 심도 있게 배울 방법을 찾습니다. 두번째 부류의 엔지니어들은 전형적으로 겉만 훑고, 기초를 이해하기보다는 특정 툴이나 기술만 익히며 기술 트렌드가 바뀔때마다 새로운 기술들만 취하죠.    
    
현재, IT산업에 뛰어드는 사람들은 급속하게 많아지고 있지만, 컴퓨터 과학 졸업생들 수는 상대적으로 그대롭니다. 이 두번째 부류 엔지니어의 과잉공급은 그들의 고용 기회를 감소시키고, 산업의 중요한 일들에서 배제시킬 것입니다. 당신이 첫번째 부류의 엔지니어가 되고 싶거나 단순히 고용 안정을 찾고 싶다면, 컴퓨터 과학을 배우는 것이 유일한 믿을구석입니다.

## 과목 가이드

### 프로그래밍
대부분의 CS 재학생들은 컴퓨터 프로그래밍에 대한 "입문"으로 시작합니다. 진짜 좋은 코스들은 초심자뿐만 아니라 처음 코딩을 배울 때 진짜 중요한 컴셉과 프로그래밍 모델을 놓친 사람들에게도 큰 도움이 됩니다. 
   
이 주제에 대한 우리의 스탠다드 추천은 바로 고전 *Structure and Interpretation of Computer Programs(번역본: 프로그램의 구조와 해석)* 입니다.(이하 SICP) [책](https://mitpress.mit.edu/sites/default/files/sicp/full-text/book/book.html)과 [MIT 비디오 강의](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-001-structure-and-interpretation-of-computer-programs-spring-2005/video-lectures/) 모두 인터넷에서 무료로 찾아볼 수 있습니다. 이 강의들도 매우 좋지만, 사실 우리가 대신 추천하고 싶은 강의는 [Brian Harvey의 SICP 강의](https://archive.org/details/ucberkeley-webcast-PL3E89002AA9B9879E?sort=titleSorter)(버클리 61A 코스용)입니다. MIT 강의들보다 좀 더 신입생에 맞춰 구성되어 있거든요.   
   
우리는 최소 SICP의 첫 세 챕터를 훑은 다음에 연습문제를 풀어보기를 추천합니다. 심화학습을 위해, [Exercism](http://exercism.io/)같은 데 있는 작은 프로그래밍 문제 세트를 풀어보세요.    
    
이 가이드가 2016년에 최초로 발행된 후에, 우리가 가장 많이 듣는 질문중에 하나는 더 최근 강의인 John DeNero가 가르친 61A의 강의 녹화본이나 그 교재인 "SICP의 기본에 맞춰" 파이썬으로 풀어낸 [Composing Programs](https://composingprograms.com/)를 추천하는지에 관한 것입니다. 우리는 DeNero의 강의도 매우 훌륭하다고 생각하고, 몇몇 학생은 그걸 더 선호하는 것 같기도 하지만, 여전히 SICP, Scheme, 그리고 Brian Harvey의 강의를 입문으로 시작하는 것을 추천합니다. 
    
왜일까요? SICP는 컴퓨터와 프로그래밍에 대한 당신의 근본적인 신념을 바꿔줄 능력(적어도 잠재력)을 갖고 있기 때문입니다. 모두가 이런 경험을 하는건 아닙니다. 어떤 사람들은 이 책을 싫어하고, 어떤 이들은 처음 몇장을 넘어가지 못할 것 입니다. 하지만 그 보답은 시도해볼만한 가치가 있죠.    
   
SICP가 별로였다면, *Composing Programs*를 시도해 보세요. 여전히 안 맞는다면, *[How to Design Programs](http://www.htdp.org/)* 를 시도해보세요. 이 중에 아무것도 노력대비 얻을 결실이 없어 보인다면, 아마 그건 다른 주제에 먼저 집중하고 한 1~2년 후쯤 다시 이 프로그래밍 훈련을 해보라는 징조일 수 있습니다. 
    
딱 말하자면, 이 가이드는 프로그래밍 생 초짜를 위해 만들어진게 **아닙니다**. 우리는 당신을 컴퓨터 과학에 대한 배경지식이 없는, 그 지식의 간극을 매우고 싶어하는 유능한 개발자로 추정합니다. 우리가 이 "프로그래밍" 섹션을 포함한 것은, 단순히 여기도 더 배울 것이 있을 거라는 조언입니다. 혹시 코딩을 한번도 해본적은 없지만, 해보고 싶은 사람이라면, [이 가이드](https://www.reddit.com/r/learnprogramming/wiki/faq#wiki_getting_started)를 참조하시기 바랍니다.
    
        
        
### 컴퓨터구조
컴퓨터 구조(때떄로 "컴퓨터 시스템", "컴퓨터 편성" 등으로 불리는)는 소프트웨어 표면 아래의 컴퓨팅에 관한 중요한 첫 단계입니다. 경험에 따르면, 독학 소프트웨어 엔지니어 사이에서 가장 괄시받는 영역이기도 하죠. 
    
우리가 제일 좋아하는 입문책은 *[Computer Systems: A Programmer's Perspective](http://csapp.cs.cmu.edu/3e/home.html)(번역본: 컴퓨터시스템, 이하 CS:APP)* 와 이 책의 챕터 1에서 6까지의 대부분을 [다루는](http://csapp.cs.cmu.edu/3e/courses.html) 상징적인 입문 컴퓨터 구조 강의입니다.
    
우리는 CS:APP의 실용적이고 개발자 중심적인 접근을 사랑합니다. 이 책에서 다루는 것보다 더 많은 컴퓨터 구조의 내용이 있음에도, 이 책은 주로 더 빠르고 효율적이며 믿을만한 소프트웨어를 만들기 위해 컴퓨터 시스템을 이해하고 싶은 사람들에게 중요한 시작점들을 제공합니다. 
    
주제에 대한 더 부드러운 접근과 하드웨어와 소프트웨어의 관계의 밸런스를 선호하는 사람에게는, *The Elements of Computing Systems(속칭 "Nand2Tetris")* 를 추천합니다. 이 책은 컴퓨터의 모든 것이 어떻게 동작하는지에 대한 완전한 이해를 시키려는 야심찬 책입니다. 각각의 챕터는 HDL의 기본 로직 게이트를 쓰는것부터 CPU와 어셈블러를 거쳐, 테트리스 게임 정도의 어플리케이션까지 전체시스템의 작은 부분을 빌딩하는것을 포함하고 있습니다.  
    
처음 여섯챕터를 읽은 후 관련 프로젝트를 수행하는 것을 추천합니다. 이는 당신이 기계의 구조와 그 위에 돌아가는 소프트웨어의 관계를 이해할도록 도울 것 입니다. 
    
전반부(와 모든 프로젝트들)는 [Nand2Tetris 웹사이트](http://www.nand2tetris.org/)에서 무료로 찾아볼 수 있습니다. [Coursera course의 비디오강의](https://www.coursera.org/learn/build-a-computer)도 있고요.
   
간결과 응집을 위해, Nand2Tetris는 깊이를 포기하였습니다. 특히, 모던 컴퓨터 구조에서 가장 중요한 두가지 컨셉인 파이프라인과 메모리 계층 구조는 이 책에서 거의 찾아볼 수 없죠.
    
Nand2Tetris의 내용이 편해졌다면, 다시 CS:APP로 돌아오거나, 훌륭한 요즘 교재인 Patterson과 Henessy의 *[Computer Organization and Design](https://smile.amazon.com/Computer-Organization-Design-Fifth-Architecture/dp/0124077269)* 를 보기를 추천합니다. 이 책의 모든 부분이 중요하진 않고, Berkeley의 [CS61C 코스](http://inst.eecs.berkeley.edu/~cs61c/sp15/)의 "Great Ideas in Computer Architecture"를 읽어보기를 추천합니다. 강의 노트와 연구는 인터넷에서 찾을 수 있고, 이전 강의들은 [인터넷 아카이브](https://archive.org/details/ucberkeley-webcast-PL-XXv-cvA_iCl2-D-FS5mk0jFF6cYSJs_)에 있습니다.

### 알고리즘과 자료구조
우리는 공통 알고리즘과 자료 구조에 정통한 것이 컴퓨터 과학 교육의 가장 중요한 부분 중 하나라는 것에 대해 수년에 걸쳐 공감하였습니다. 이는 모든 학습 영역에서 통용되는 일반적인 문제 풀이 능력을 기르는 것에도 큰 도움이 되죠.
    
세상엔 수백개의 책이 있지만, 우리의 추천은 Steven Skiena가 쓴 *[The Algorithm Design Manual](https://smile.amazon.com/Algorithm-Design-Manual-Steven-Skiena/dp/1848000693/)* 입니다. Skiena는 확실히 알고리즘 문제 풀이를 사랑하며 그의 학생과 독자들에게 같은 열정을 키우게 하는데 성공하였습니다. 우리 의견은, CLRS와 Sedgewick과 같은 더 많이 추천되는 책들은 주로 실용적인 문제풀이 학습하는 사람들에게는 너무 무거운 경향이 있습니다. 
    
비디오 강의를 선호하는 사람들은 [Skiena의 무료 온라인 강의](https://www.youtube.com/watch?v=A2bFN3MyNDA&list=PLOtl7M3yp-DX32N0fVIyvn7ipWKNGmwpp)를 보세요. 우리는 [Coursera](https://www.coursera.org/specializations/algorithms)나 [다른데](http://timroughgarden.org/videos.html)서 볼 수 있는 Tim Roughgarden의 강의도 매우 좋아합니다. Skiena 강의와 Roughgarden의 강의에 대한 선호는 개인 취향에 따릅니다. 사실, 수십개의 다른 좋은 매터리얼도 있으니, 만약 좋아하는걸 찾았다면, 그걸로 공부하시기 바랍니다!
    
실습을 위해, 우리는 [Leetcode](https://leetcode.com/)의 문제풀이를 추천합니다. 이 사이트에는 흥미로운 문제들과 함께 멋진 솔루션과 토론을 볼 수 있어요. 유수의 소프트웨어 회사들의 기술 면접에서 널리 사용되는 문제들에 대한 내 실력도 체크할 수 있습니다. 공부하면서 100개 정도의 랜덤 Leetcode 문제들을 풀어보기를 추천합니다.
    
마지막으로, 일반적은 문제 해결에 있어서 훌륭하고 독창적인 가이드인 *[How to Solve It](https://smile.amazon.com/How-Solve-Mathematical-Princeton-Science/dp/069116407X/)* 을 강력 추천합니다. 이 책은 수학에 뿐만 아니라 컴퓨터 과학에도 적용 가능합니다.
     
### 컴퓨터 과학을 위한 수학
어떤면에서, 컴퓨터 과학은 응용 수학의 한 부분이 아주 커진 것과 같습니다. 많은 소프트웨어 엔지니어들이 이를 무시하려 하지만(어느정도는 성공한 듯 하지만), 우리는 정공법으로 공부하여 받아들이기를 추천합니다. 이걸 성공하면 다른 사람들에 비해 엄청난 경쟁력을 갖추게 될 것입니다.
    
CS를 위한 수학에 있어 가장 관련 깊은 영역은 "이산수학"인데, "이산"은 "연속"의 반댓말이며 미적분학에서 벗어난 흥미로운 응용 수학의 집합체와 같습니다. 모호한 정의를 고려하면, "이산수학"의 모든 부분을 이해하려고 하는 것은 의미 없습니다. 좀 더 현실적인 목표는 논리학, 조합론과 확률, 집합 이론, 그래프 이론, 유익한 암호학 이론 몇개를 익히는 것 입니다. 선형대수는 컴퓨터 그래픽스와 머신 러닝에서의 중요성을 고려하면 또다른 공부 해 볼만한 분야입니다.
    
이산수학 공부의 시작은 [László Lovász의 강의노트](https://cims.nyu.edu/~regev/teaching/discrete_math_fall_2005/dmbook.pdf) 세트를 추천합니다. Lovász 교수는 접근하기 쉽고 학습적인 컨텐츠를 잘 만들어 냈고, 이는 교재보다 더 좋은 시작 포인트를 제공합니다. 
    
심화 학습을 위해, *[Mathematics for Computer Science](https://courses.csail.mit.edu/6.042/spring17/mcs.pdf)* 와 책 동명의 MIT 강의 노트를 추천합니다. [비디오 강의](https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-042j-mathematics-for-computer-science-fall-2010/video-lectures/)도 온라인에서 무료로 제공되며, 이산수학 학습을 위해 추천합니다.
    
선형대수는 [선형대수 기초](https://www.youtube.com/playlist?list=PLZHQObOWTQDPD3MizzM2xVFitgF8hE_ab) 강의로 시작하여 Gilbert Strang의 [책](https://www.amazon.com/Introduction-Linear-Algebra-Gilbert-Strang/dp/0980232775/)과 [강의](https://ocw.mit.edu/courses/mathematics/18-06-linear-algebra-spring-2010/video-lectures/)로 진행하기를 추천합니다.
    
### 운영체제
*[Operating System Concepts(번역본: 운영체제)](https://www.amazon.com/dp/1118063333/)*(속칭 "공룡책")와 *[Modern Operating Systems(번역본: 운영체제론)](https://www.amazon.com/dp/013359162X/)* 은 운영체제의 "고전"입니다. 두 책 모두 명백함의 부족과 학생들에게 불친절한 내용으로 비판을 받고 있죠.
    
*Operating Systems: Three Easy Pieces(번역본: 운영체제 아주 쉬운 세가지 이야기, 이하 OSTEP)* 는 인터넷에서 [무료로 찾아볼 수 있는](http://pages.cs.wisc.edu/~remzi/OSTEP/) 좋은 대안입니다. 이 책의 구조와 가독성이 특히 좋고, 문제들은 풀어 볼 가치가 있습니다. 
    
OSTEP을 다 봤으면, 우리는 "{ㅇㅇ운영체제} 살펴보기" 같은 이름의 책으로 특정 운영체제의 설계 결정(design decisions)을 탐구해보기를 추천합니다. 예를들어, *[Lion's commentary on Unix](https://www.amazon.com/Lions-Commentary-Unix-John/dp/1573980137/)*, *[The Design and Implementation of the FreeBSD Operating System](https://www.amazon.com/Design-Implementation-FreeBSD-Operating-System/dp/0321968972/)* 와 *[Mac OS X Internals](https://www.amazon.com/Mac-OS-Internals-Systems-Approach/dp/0321278542/)* 같은 책으로 말입니다. Linux용으로는 Robert Love의 환상적인 [Linux Kernel Development](https://www.amazon.com/Linux-Kernel-Development-Robert-Love/dp/0672329468)를 추천합니다.
    
운영체제에 대한 이해를 정리하는 가장 좋은 방법은 작은 커널의 코드를 읽어보고 기능을 더해보는 것입니다. 그 중 [xv6](https://pdos.csail.mit.edu/6.828/2016/xv6.html)는 ANSI C와 x86의 Unix V6 포트로, MIT 강의를 위해 유지되고 있습니다. OSTEP은 추후 프로젝트를 위한 엄청난 아이디어로 가득찬 [xv6 연구](http://pages.cs.wisc.edu/~remzi/OSTEP/lab-projects-xv6.pdf)를 부록으로 실었습니다.
    
### 컴퓨터 네트워킹
많은 소프트웨어 엔지니어링이 웹서버와 클라이언트에 있다는 것을 고려하면, 당장 가장 가치있는 컴퓨터과학 중 하나는 컴퓨터 네트워킹입니다. 네트워크를 체계적으로 공부한 독학생들은 수년간 들어왔던 용어, 개념과 프로토콜을 드디어 이해할 수 있을겁니다.
    
우리가 가장 좋아하는 책은 *[Computer Networking: A Top-Down Approach(번역본: 컴퓨터 네트워킹 하향식 접근)](https://smile.amazon.com/Computer-Networking-Top-Down-Approach-7th/dp/0133594149/)* 입니다. 이 책의 미니 프로젝트들과 문제풀이는 해볼 가치가 있고, 책에서 온라인에 제공한 ["Wireshark labs"](http://www-net.cs.umass.edu/wireshark-labs/)가 특히 좋습니다.
    
비디오 강의를 선호하는 사람들에게는 예전엔 스탠포드의 MOOC 플랫폼인 Lagunita를 통해 제공되었지만, 슬프게도 이제는 유튜브의 비공식적인 플레이리스트로밖에 볼 수 없는 스탠포드의 *[Introduction to Computer Networking course](https://www.youtube.com/playlist?list=PLvFG2xYBrYAQCyz4Wx3NPoYJOFjvU7g2Z)* 를 추천합니다.

### 데이터베이스
데이터베이스 시스템은 다른 주제보다 더 독학하기 힘듭니다. 꽁꽁 숨겨진 상업적인 인센티브를 위한 아이디어가 많은 상대적으로 최신(1970년대 이후) 학문이죠. 추가적으로, 많은 잠재적인 훌륭한 교재 저자들은 회사로 들어갔거나 창업하기를 선호하였습니다.
    
이런 상황을 고려해 우리는 독학생들이 교재보다는 Berkeley의 Joe Hellerstein의 데이터베이스 강의인 [CS186 강의 녹화본](https://www.youtube.com/user/CS186Berkeley/videos)으로 시작한 후 논문들을 읽어보기를 추천합니다.
    
입문자들에게 추천할만한 책은 관계형 데이터베이스(RDBMS)가 어떻게 동작하는지를 높은 수준으로 풀어낸 "[Architecture of a Database System](http://db.cs.berkeley.edu/papers/fntdb07-architecture.pdf)"를 추천합니다. 이는 추후 공부하는데 유용한 뼈대가 될 것 입니다.
    
소위 데이터베이스 "[레드북](http://www.redbook.io/)"으로 불리는 *Readings in Database Systems* 은 Peter Bailis, Joe Hellerstein와 Michael Stonebraker가 엮어내고 편집한 컬렉션입니다. CS186의 내용에서 더 심화한 내용을 학습하고 싶다면, 레드북이 바로 다음 스텝입니다.
    
만약 꼭 입문 교재를 보고 싶다면, Ramakrishnan와 Gehrke가 쓴 *[Database Management Systems](https://smile.amazon.com/Database-Management-Systems-Raghu-Ramakrishnan/dp/0072465638/)* 를 추천합니다. 많은 심화 학생들에게, Jim Gray의 고전 *[Transaction Processing: Concepts and Techniques](https://www.amazon.com/Transaction-Processing-Concepts-Techniques-Management/dp/1558601902)* 도 가치가 있지만, 입문서로는 추천하지 않습니다.

마지막으로, 데이터 모델링은 데이터베이스로 일할 때 가장 괄시받고 대충 는 영역입니다. 우리의 추천은 *[Data and Reality: A Timeless Perspective on Perceiving and Managing Information in Our Imprecise World](https://www.amazon.com/Data-Reality-Perspective-Perceiving-Information/dp/1935504215)* 입니다.

### 언어와 컴파일러
대부분의 프로그래머는 언어를 배우는 반면, 대부분의 컴퓨터 과학자들은 언어에 대해 배웁니다. 이는 컴퓨터 과학자들에게 프로그래머 대비 뚜렷한 이점을 줍니다. 하물며 프로그래밍 영역에서도요! 이들의 지식은 일반화됩니다. 이들은 특정 언어를 배우기만 한 사람들에 비해 새로운 언어의 동작을 좀 더 깊이 빨리 이해할 수 있습니다.
    
우리가 추천하는 입문 교재는 인터넷에서 볼 수 있는 Bob Nystrom의 훌륭한 *[Crafting Interpreters](https://craftinginterpreters.com/contents.html)* 입니다. 이 책은 잘 정리되어 있고, 대단히 재미있으며 언어와 언어도구를 더 잘 이해하고 싶어하는 것이 주요 목표인 사람에게 잘 맞습니다. 당신의 흥미를 유지시키는 어떤 "도전"이던 시도하며 모든 내용을 시간내어 살펴보기를 추천합니다.
      
가장 전통적인 추천은 "드래곤북"이라고 불리는 *[Compilers: Principles, Techniques & Tools(번역본: 컴파일러)](https://smile.amazon.com/Compilers-Principles-Techniques-Tools-2nd/dp/0321486811)* 입니다. 아쉽게도, 이 책은 독학용이라기 보다는 1-2학기용 코스를 위한 주제가 있는 강사용입니다.

드래곤북을 보기로 결정했다면, 가능한 멘토와 함께, 중요한 주제들을 선별하는것이 필요합니다. 사실, 우리가 추천하는 드래곤북 활용법은, 비디오 강의의 보충 교재로 활용하는 것입니다. [edX의 Alex Aiken의 강의](https://www.edx.org/course/compilers)를 추천합니다.

### 분산시스템
컴퓨터 수가 증가하면서, 영역도 넓어졌습니다. 이전의 사업들이 큰 메인프레임을 사려했던 반면, 이제는 아주 작은 어플리케이션도 다양한 기기에서 실행되는것이 일반적입니다. 분산시스템은 이러한 경향에 관련된 장단점을 설명하는 학문입니다.

독학용 책으로는 Martin Kleppmann의 *[Designing Data-Intensive Applications(이하 DDIA)](https://smile.amazon.com/Designing-Data-Intensive-Applications-Reliable-Maintainable-ebook/dp/B06XPJML5D/)* 를 추천합니다. DDIA는 전통 교재보다 훨씬 뛰어나며 어쨌거나 깊이나 디테일을 포기하고 싶지 않은 실용주의자들을 위해 고안되어 가독성이 뛰어납니다.

좀 더 전통적인 책을 찾는, 혹은 온라인에서 무료로 볼 수 있는 책을 선호하는 사람들에게는 Maarten van Steen와 Andrew Tanenbaum의 *[Distributed Systems, 3rd Edition](https://www.distributed-systems.net/index.php/books/ds3/)* 를 추천합니다.

비디오 강의를 선호하는 사람들에게는, 온라인에서 찾아볼 수 있는 훌륭한 Robert Morris의 대학원 강의인 [MIT의 6.824](https://www.youtube.com/watch?v=cQP8WApzIQQ&list=PLrw6a1wE39_tb2fErI4-WkMbsvGQk9_UB)와 [자료](https://pdos.csail.mit.edu/6.824/schedule.html)를 추천합니다.

교재나 보조자료를 뭘 선택했던, 분산시스템을 공부하려면 논문을 읽는 것은 필수입니다. 추천 리스트를 참조하시고, 지역 [Papers We Love](https://paperswelove.org/chapter/seoul/) 챕터에 참여하시기를 추천합니다.

## 자주 묻는 질문
#### 이 가이드의 대상은 누구인가요?
독학 엔지니어, 부트캠프 졸업생 혹은 선행하는 고등학교 졸업생, 혹은 대학 강의를 보조할 독학 컨텐츠를 찾는 대학생을 염두에 두었습니다. 이 과정을 언제 시작해야 하냐는 질문은 전적으로 개인에 달렸으나, 대부분의 사람들은 CS 이론을 깊이 이해하기 전에 직업 경험을 갖는 경향이 있습니다. 예를 들어, 직장에서 데이터베이스로 일하는 사람들이 데이터베이스 시스템을 공부하고 싶어하며, 한 두개의 웹 프로젝트를 한 사람들이 컴퓨터 네트워킹을 좋아합니다.

#### AI/그래픽/ㅇㅇㅇ는요?
우리는 모든 숙련된 소프트웨어 엔지니어가 전공이나 산업에 관계 없이, 하지만 시스템에 집중하여 알아야 할 컴퓨터 과학 주제들로 목록을 한정지었습니다. 경험에 의하면, 이것들이 독학 엔지니어들과 부트캠프 졸업생들에게 가장 투자대비 얻을 것이 많은 주제이며, 추후 학습에 단단한 기반이 됩니다. 결과적으로, 교재나 논문을 더 쉽게 고를수 있고 다른 가이드 없이 주요 개념을 익힐 수 있을 것입니다. 여기 그 "선택과목"에 대한 우리의 몇몇 입문용 추천입니다:
* 인공지능 : [Berkeley의 인공지능 입문 과정](http://ai.berkeley.edu/)의 비디오 강의를 듣고 Pacman 프로젝트를 완성하세요. 교재로는, Russel과 Norvic의 *Artificial Intelligence: A Modern Approach* 를 추천합니다.
* 머신러닝 : Andrew Ng의 Coursera 과정을 들으세요. 인내심있게, 딥러닝의 새로운 주제들을 배우기 전에 기본에 대해 확실히 익힐 수 있도록 하세요.
* 컴퓨터 그래픽 : [Berkeley의 CS 184](http://inst.eecs.berkeley.edu/~cs184/fa12/onlinelectures.html) 컨텐츠를 살펴보고, 교재로는 [Computer Graphics: Principles and Practice](https://www.amazon.com/Computer-Graphics-Principles-Practice-3rd/dp/0321399528)를 추천합니다.

#### 추천하신 순서가 꼭 따라야 하나요?
현실적으로, 모든 주제들이 다 많이 공통되는 부분이 있고, 서로 서로 영향을 미칩니다. 예를 들어 이산수학과 알고리즘의 관계를 봅시다. 수학을 공부하는 것이 알고리즘을 더 심화있게 이해하는데 도움을 주고, 알고리즘을 배우는 것은 이산수학에 동기와 맥락을 부여할 것입니다. 이상적으로, 이 주제들을 커리어동안 여러번 다시 훑어보세요.    
    
마찬가지로, 우리가 추천하는 순서는 단순히 *시작하기 위해서* 입니다. 만약 어떤 이유로 다른 순서로 공부하고 싶다면, 그렇게 하세요. 우리 생각에 중요한 "선후관계"는, 운영체제나 데이터베이스 전에 컴퓨터 구조를 배우는 것이며, 분산시스템을 배우기 전에 네트워킹과 운영체제를 익히는 것입니다.

#### Open Source Society나 freeCodeCamp의 커리큘럼과 다른점은 뭔가요?
이 가이드가 2016년에 처음 쓰여졌을 때, 이 [OSS 가이드](https://github.com/open-source-society/computer-science)는 주제도 너무 많고, 별로인 컨텐츠도 소개하였으며, 어떤 과정이 왜 또는 어떤 면이 가치 있는지에 대한 이론적 해석이나 가이드도 없었습니다. 우리는 소프트웨어 엔지니어라면, 전공에 관계 없이 반드시 알아야할 과정들로 리스트를 제한하기 위해 애썼으며, 왜 각각의 과정들이 포함되었는지 이해시키려고 하였습니다. 향후 몇년간, OSS 가이드는 발전해왔지만, 이 가이드가 좀 더 명확하고 결집된 가이드를 제공한다고 생각합니다.

freeCodeCamp는 주로 컴퓨터 과학이 아닌 프로그래밍에 집중합니다. 왜 컴퓨터 과학을 배워야 하는지 궁금하다면, [위](#왜-컴퓨터-과학을-배워야-하는가?)를 참조하세요. 만약 처음 프로그래밍을 배우는거라면, 먼저 거기에 집중하고 1-2년 후에 다시 이 가이드를 참조하는 것을 추천합니다.

#### ㅇㅇ 언어는요?
특정 언어를 배우는 것은 컴퓨터 과학의 특정 분야를 배우는것과는 아예 다른 얘기입니다.(언어 하나를 배우는 것이 더 쉽고 덜 가치 있죠.) 당신이 이미 몇몇 언어를 알고 있다면, 이 가이드를 따라 배운 언어를 사이사이에 매워 넣거나 나중을 위해 내버려 두는것을 강력하게 추천합니다. 당신이 프로그래밍을 잘 배워놨다면(*Structure and Interpretation of Computer Programs* 같은 걸로), 그리고 특히 컴파일러를 잘 익혔다면, 새로운 언어의 기본을 익히는데 주말 정도면 충분하여 직장에서는 라이브러리/도구/에코시스템을 익힐 수 있을 것입니다.

#### 요즘 뜨는 ㅇㅇ 기술은요?
어떤 단독 기술도 학습의 주요 파트가 되어 배워야 할 만큼 중요하지 않습니다. 반면에, 당신이 새로운 것을 배우고 싶어한 다는 것은 훌륭합니다. 팁은 그 요즘 뜨는 기술이 큰 그림에 어떻게 맞는지 살피기 전에 특정기술의 기반 분야나 개념으로 돌아와 심도 있게 학습하는 것입니다.

#### 왜 아직도 SICP를 추천하나요?
그냥 한번 시도해 보세요. 어떤 사람들은 SICP가 완전 쩌는, 다른 책에서는 거의 찾아볼 수 없는 특성을 가졌다고 생각합니다. 만약에 별로였다면, 다른 것들을 먼저 시도해본 후 다시 SICP로 돌아올 수도 있죠.

#### 왜 아직도 드래곤북을 추천하나요?
드래곤북은 여전히 컴파일러를 위한 가장 완전한 싱글 컨텐츠입니다. 이 책이 파싱과 같은 요즘 트렌드엔 맞지 않는 특정 주제들을 과하게 강조해 나쁜 평가를 받긴 합니다. 중요한 건, 이 책은 처음부터 끝까지 다 보라고 만들어진게 아니라, 강사들이 강의를 구성할 때 이용할 수 있도록 충분한 매터리얼을 제공하는 것입니다. 비슷하게, 독학생들도 책의 이점들만 취하거나, 강사들이 공개 강의에서 공유한 과정개요를 참조할 수도 있습니다.

#### 책들은 어떻게 싸게 구할 수 있나요?
우리가 추천한 책들은, 저자들에게 감사하게도, 온라인에서 많이 찾아볼 수 있습니다. 그렇지 않은 것들은, 예전 에디션의 중고책을 사기를 추천합니다. 보통 교재가 여러 에디션이 있으면, 이전 에디션도 꽤 볼만 합니다. 가격차이가 10배 난대도, 새로운 에디션이 이전 것보다 10배 좋거나 한게 아니더라구요!

#### 누가 이 가이드를 썼나요?
이 가이드는 본래 [Oz Nova](https://twitter.com/oznova_)와 [Myles Byrne](https://twitter.com/quackingduck)가 썼고, Oz가 2020년에 업데이트했습니다. 이 가이드는 샌프란시스코의 소규모 그룹과 온라인 라이브에서 1000명이 넘는 독학 엔지니어들과 부트캠프 졸업생들을 가르쳤던 경험에 의거하였습니다.

우리는 당신이 위의 주제들을 충분한 시간과 동기만 있다면 충분히 독학할 수 있을거라 확신합니다. 하지만 좀 더 인텐시브하고, 구조적이며, 교수자가 이끄는 프로그램을 선호한다면, 우리의 [Computer Science Intensive](https://bradfieldcs.com/csi/) 코스도 괜찮습니다. 우리는 **[절대](https://ozwrites.com/masters/)** 석사학위를 따는 것을 추천하지 않습니다.

이 가이드에 대한 업데이트나 컴퓨터 과학 뉴스와 리소스를 받아보고 싶은 사람은, Bradfield의 메일링 리스트에 참여하세요. [원문 페이지](https://teachyourselfcs.com/)의 최하단에서 구독할 수 있습니다.
