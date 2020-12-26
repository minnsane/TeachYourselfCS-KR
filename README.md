# 컴퓨터과학 스스로 학습하기

노트 : 이 가이드는 2020년 5월에 확장 업데이트 되었습니다. 이전 버전은 [여기](https://teachyourselfcs.com/2016/)를 참조해주세요.

만약 당신이 독학 엔지니어나 부트캠프 졸업생이라면, 컴퓨터 과학을 배우는 것도 놓쳐서는 안됩니다.   
다행스럽게도, 시간이나 학위를 위한 학자금 투자 없이 월드클래스 컴퓨터과학(Computer Science, 이하 CS) 교육을 받을 수 있습니다.💸
      
세상엔 수많은 리소스가 있지만, 어떤 것들은 다른 것들보다 더 뛰어납니다. 당신에겐 '200개가 넘는 무료 온라인 코스' 같은 리스트는 필요 없습니다. 다음 질문에 답만 있으면 됩니다:
* **어떤 과목**을 배워야 하며, 왜 배워야 하는가?
* 각 과목 **최고의 책 또는 영상 강의**는 무엇인가?   

이 가이드는 이러한 질문에 확실한 답을 주기 위한 우리의 시도입니다.   

## 요약
아래의 아홉 과목을 대략적으로 나열된 순서대로 추천 도서나 강의를 통해(둘 다 보는게 이상적) 학습하세요.
각 과목당 100-200시간 정도 투자하여 공부하고, 나중에 일할면서 필요할때 다시 찾아보세요.🚀

|과목|왜 공부해야 하는가?|책|영상|
|---|--------------|-|---|
|[프로그래밍](#프로그래밍)|재귀 같은 걸 "완전히 이해하지는 못한" 사람이 되지 마세요.|Structure and Interpretation of Computer Programs|Brian Harvey’s Berkeley CS 61A|
|[컴퓨터구조](#컴퓨터구조)|컴퓨터가 실질적으로 어떻게 작동하는 지에 관한 확실한 멘탈모델이 없다면, 더 높은 단계의 추상화는 다루기 힘들겁니다.|Computer Systems: A Programmer's Perspective|Berkeley CS 61C|
|[알고리즘과 자료구조](#알고리즘과-자료구조)|스택, 큐, 트리나 그래프 같은 항상 보이는 자료구조에 대한 이해가 없다면, 문제 풀이는 할 수 없을 것입니다.|The Algorithm Design Manual|Steven Skiena’s lectures|
|[CS를 위한 수학](#CS를-위한-수학)|컴퓨터 과학이 본래 응용수학의 탈주 브랜치인만큼, 수학을 배워 경쟁력을 높일 수 있습니다.|Mathematics for Computer Science|Tom Leighton’s MIT 6.042J|
|[운영체제](#운영체제)|당신이 짠 코드 대부분은 운영체제에 의해 실행되니, 어떻게 상호작용하는지 알아야합니다.|Operating Systems: Three Easy Pieces|Berkeley CS 162|
|[컴퓨터 네트워킹](#컴퓨터-네트워킹)|인터넷은 매우 중요해졌습니다. 어떻게 동작하는지 이해하고 그 엄청난 잠재력을 깨워보세요.|Computer Networking: A Top-Down Approach|Stanford CS 144|
|[데이터베이스](#데이터베이스)|데이터베이스는 대부분의 중요한 프로그램의 핵심이지만, 어떻게 동작하는지 제대로 이해하는 사람은 거의 없습니다.|Readings in Database Systems|Joe Hellerstein’s Berkeley CS 186|
|[언어와 컴파일러](#언어와-컴파일러)|언어와 컴파일러가 실제 어떻게 동작하는지 이해한다면, 더 나은 코드를 작성하고 새로운 언어를 쉽게 배울 수 있습니다.|Crafting Interpreters|Alex Aiken’s course on edX|
|[분산시스템](#분산시스템)|요즘은 *대부분*의 시스템이 분산시스템입니다.|Designing Data-Intensive Applications by Martin Kleppmann|MIT 6.824|

## 그래도 너무 많죠?
9개 과목을 몇년동안 자습해야 한다는 사실이 너무 부담스럽다면, 두 가지 책에 집중하기를 추천 드립니다: *Computer Systems: A Programmer's Perspective(번역본: 컴퓨터시스템)*과 *Designing Data-Intensive Applications(번역본: 데이터 중심 애플리케이션 설계)*. 우리가 경험해 본 바, 이 두 책이 특히 네트워크 어플리케이션 관련된 일을 하는 독학 엔지니어와 부트캠프 졸업생에게 들인 시간 대비 고효율을 제공합니다. 이 책들은 위 리스트의 다른 주제들을 위한 맛보기가 되기도 할 거에요.

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
    
Nand2Tetris의 내용이 편해졌다면, 다시 CS:APP로 돌아오거나, 훌륭한 요즘 교과서인 Patterson과 Henessy의 *[Computer Organization and Design](https://smile.amazon.com/Computer-Organization-Design-Fifth-Architecture/dp/0124077269)* 를 보기를 추천합니다. 이 책의 모든 부분이 중요하진 않고, Berkeley의 [CS61C 코스](http://inst.eecs.berkeley.edu/~cs61c/sp15/)의 "Great Ideas in Computer Architecture"를 읽어보기를 추천합니다. 강의 노트와 자료는 인터넷에서 찾을 수 있고, 이전 강의들은 [인터넷 아카이브](https://archive.org/details/ucberkeley-webcast-PL-XXv-cvA_iCl2-D-FS5mk0jFF6cYSJs_)에 있습니다.


