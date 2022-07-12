#지라 내용 정리

## 스크럼
```
스크럼 프로젝트 
  - Jira의 Scrum을 활용해서 설계가 끝나고 개발에 들어갔을 때 할일을 백로그로 생성할 수 있다. 
  
우선순위 설정 
  - 백로그 우선순위를 설정하여 정렬하는 것은 회사차원에서 관리에서 사용 가능한 방법이다. 
    팀에서는 그냥 드래그롤 정렬해야한다. 

추정(estimation)
  - 스크럼에서 추정은 개별항목을 완성하는데 어느정도가 걸릴지를 대략적으로 추정하는 것이다. 
    jira에서 추정방식은 3가지가 있다. 여기서 팀방식은 Story point만 지원하고 
    회사방식은 3가지 모두 지원한다.
    
	1. Stroy Point 
      - 해당 이슈를 수행하는데 다른 이슈에 비해 상대적으로 어느정도 노력해야할지에 대해서 대략적인 숫자로 판단하는 방식
	    스토리 포인트도 잘 모르는 이해 당사자들이 보게 되면 스토리 포인트에 부여한 숫자는 해당 업무를 수행하는데 드는 시간 
		단위로 이해하는 경우가 많다. 하지만 스토리 포인트의 숫자단위는 업무 소요 예상 시간과는 관련이 없다. 
		스토리 포인트는 피보나치 수열을 사용한다. 
		
		추가 참고 자료 
		  - https://engineering.linecorp.com/ko/blog/user-story-point-in-line-pay-team/
	2. 최초 추정 시간 
	3. 이슈 개수
	
	스프린트 마다 스토리포인트를 이슈마다 부여하면 총 스토리 포인트가 존재할 텐데 이런 추정치는 팀원수를 기반으로 
	다음 스프린트에 추가해야할 작업의 양을 측정하는데 도움이 된다. 첫 스프린트를 생성할 때 한 스프린트마다 
	얼마의 스토리 포인트를 부여할지 알 수 없지만 몇번의 스프린트 후에 팀은 각 스프린트에서 수행할 수 있는
	작업의 양을 잘 파악할 수 있으므로 스프린트 계획시 과도하거나 무리한 계획을 잡아서 스프린트가 깨지는 것을 
	방지해야 한다. 

스프린트 시작 및 모니터링, 종료하기 
  - 스프린트를 시작하기를 눌러 스프린트를 진행하면 가장 중요한 이벤트중 하나인 daily standup meeting을 시행할 수 있다.
    이 때 전날 할일과 오늘 할일, 진행을 가로막고 있는 일에 대해서 공유를 할 수 있다. 진행을 시작한 이슈는 보드에서 진행중인 칸반으로 
	옮겨놓고 완료한 이슈는 완료 칸반으로 옮기면 된다.
  - 스프린트에서 가장 중요하게 강조하는 것 중에 하나는 스프린트 기간 내에 새로운 업무를 받지 않는 것이다. 정해진 기간안에 정해진 
    업무를 통해 제품 증분을 만들어 내는 것이 목표이기 때문에 새로운 업무는 스프린트를 깨지게 하는 경우가 많다. 

  - 스토리포인트보다 더 도움이되는 정보는 여러가지 보고서이며 그중에 대표적인 보고서는 번다운차트이다.
    번다운 차트 
	  - 추정한 스토리 포인트와 현재 처리된 스토리 포인트를 그래프로 표시해서 프로젝트 진행 사항에 대해서 명확하게 인지할 수 있다.
	
  스프린트 리뷰 미팅 
    - 스프린트에서 만들어낸 제품 증분의 기능성에 대한 검토와 조정을 하는 단계이다.
  스프린트 회고 미팅 
    - 스프린트 리뷰 미팅 후에는 스프린트 회고 미팅을 진행한다. 스프린트 회고는 프로세스와 환경에 대해서 검토하고 조정하는 것인데
	  스프린트 기간동안 무엇이 좋았고 무엇을 개선해야 하는지에 대해서 토론하는 것이다. 이때 주의할 점은 스프린트에 발생하는 문제에 
	  집중하는 경우가 많은데 이럴 경우 회고 미팅을 굉장히 소극적이고 부정적으로 대하게될 소지가 많으니 긍정적인 내용에 대해서 할 것을 
	  권장하고 있다. 컨플루언스를 사용한다면 컨플루언스에서 회고록 템플릿을 제공하므로 활용하면 좋다.
	  컨플루언스에 space를 생성해서 회고록 페이지를 템플릿을 이용해서 만들고 회고록 작성시마다 하위 페이지를 생성해서 추가하면 회고록이 
	  쌓이는 것을 확인할 수 있다. 
```

## 칸반 
```
칸반
  - 칸반은 신호 카드를 의미하는 일본어로 어떤 일을 할 수 있는 상태인지 알려주는 것 
  - 스크럼처럼 다양한 이벤트와 절차, 산출물을 정의하지 않으나 시각화와 2가지 중요한 규칙이 있음
  - 칸반 보드에서 프로세스의 흐름을 이해하고 병목지점을 파악해서 프로세스와 업무를 개선할 수 있음
  
  제약 1. 
    - 개발팀은 당김(pull)방식으로 일을 가져옴
  제약 2. 
    - 진행중 작업 갯수 제한 
  
  - 칸반은 스크럼과 달리 번다운 차트 대신 누적흐름도를 주요 지표로 사용합니다.
    누적흐름도는 시간별, 상태별 이슈 개수와 진행과정이 표시되며 팀의 흐름을 유지하고 개선하기 위한 기반 데이터를 제공한다.

스크럼과 칸반은 비슷하지만 가장 큰 차이점은 출시 주기와 역할 제약조건의 유형에 차이가 있다. 스크럼은 진행중 업무 제약 조건을 위해서 
스프린트라는 1~4주 단위의 시간제약을 사용하고 스프린트에 영향을 줄만한 변경 사항을 받지 않는다.
칸반은 동시에 진행중인 업무의 수를 제한해서 제약조건을 둔다. 역할 부분에 있어서 스크럼은 세가지 역할을 정의하지만 칸반은 그런 제약이 
존재하지 않는다. 스크럼은 스프린트 계획 미팅, 일일 미팅, 스프린트 회고 미팅 등 다양한 이벤트를 정의하지만 칸반은 그런 이벤트에 대한 
제약이 존재하지 않는다. 
```

# PO(Project Owner)에게 유용한 기능 
```
Version과 Release 관리 
  Version
    - 프로젝트의 특정 시점의 결과물을 의미하며, 여러 개선사항이나 버그 수정 등을 논리적으로 묶은 단위로 
      목표 릴리즈 날짜가 있으므로 프로젝트의 수행 일정을 파악할 수 있다.
  - version과 release를 가지고 jira에서 칸반 프로젝트로 일정관리 뿐만 아니라 프로젝트 관리도 할 수 있다.

Release note 만들기 
  - 프로젝트에 만든 버전과 릴리스 정보를 활용해서 고객에게 전달할 Release note를 만드는 법을 학습
```
