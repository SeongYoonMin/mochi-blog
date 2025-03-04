# MOCHI BLOG
모찌 블로그는 React와 Nextjs에 대해 깊게 공부할 겸 직접 블로그를 운영해 보고자 시작한 프로젝트입니다.

## Skill Set
front : Next.js(react)<br/>
back : Nestjs<br/>
Server State : tanstack/react-query<br/>
Client State : Zustand<br/>
CSS: tailwindcss, class-variance-authority<br/>
UI Library: shadcn/ui<br/>
DB: Supabase(postgreSQL)<br/>
ORM: prisma<br/>

## 스킬 선택 이유
### Next.js
Next.js는 현재 가장 많이 선택반은 React로 제작된 Javascript Framework입니다. 또한 React와 다르게 서버 사이드 렌더링을 기본적으로 제공합니다. 

그로 인해 React를 이용한 방식보다 빠른 페이지 로딩속도와 SEO 최적화를 제공해줍니다. 또한 파일 시스템 기반의 자동 라우팅을 통해 별도의 라우팅을 설정하지 않아도 폴더의 설계에 따라 자동으로 라우팅을 제공합니다. 

위와 같은 이유로 저는 Next.js를 택하였습니다.
> 무조건 장점만 있는건 아니라고 생각합니다. 하지만 제가 당장 느끼기에는 단점보다는 장점이 더 크게 와닿아서 택하게 되었습니다.

### Nestjs
Nestjs는 Node.js를 기반으로 만들어진 서버 프레임워크입니다. Next.js에도 API routes와 같은 서버리스 를 지원하는데 왜 Nestjs를 택하였냐면 저는 사실 서버에 대해 크게 잘 알지못하지만, javascript로 완벽하게 백엔드를 지원할 수 있는 프레임워크라고 생각하였기 때문에 Nestjs를 택하였습니다.

### tanstack/react-query
server state 없이도 개발을 할 수는 있지만, react-query와 같은 라이브러리를 사용하지않고 직접 해당 상태에 대한 처리를 구현하려면 너무 많은 시간과 리소스가 낭비된다 생각하여 react-qeury를 사용하기로 결정하였습니다.

### Zustand
Zustand는 제가 찾아본 React의 state management중 가장 간단하고 사용하기 편하다고 느꼈습니다. 불필요한 셋팅을 최소한으로 하고, 간편한 호출 방식등 많은것들이 와닿았습니다. 또한 저는 vue의 pinia를 기존에 많이 사용하였는데 그런 pinia와 사용방식이 가장 유사하다고 생각하여 선택하였습니다.

### tailwindCSS
tailwindcss는 매우 사랑받고 있는 css framework중 하나입니다. styled-component나 emotion등을 사용해서 구현할 수 있지만 css나 styled를 사용하여 컴포넌트 내부에서 선언해줘야하고, CSS와의 분리가 힘들다고 생각하였습니다. 또한 후술할 cva나 shadcn/ui와 같은 라이브러리와도 호환성이 매우 좋고 더 편리하게 사용할 수 있다고 생각하여 택하였습니다.

### Class Variance Authority
ClassVarianceAuthority(이하 cva)는 tailwindcss의 큰 단점중 하나인 너무나도 긴 클래스명과 optional한 style을 고려하기 위해 택한 라이브러리입니다. 해당 라이브러리를 이용하여 tailwindcss를 보다 유연하게 사용할 수 있어 선택했습니다. 

### shadcn/ui
shadcn/ui는 headlessUI로써 기본적으로 페이지 구현에 필요한 애니메이션이나 여러 효과들(메뉴, 사이드바 등등) 에 대한 구현을 고민할때 알게된 라이브러리입니다. 직접 구현하려면 많은 시간과 리소스를 사용해요하고 또한 그 구현파일들이 최적의 구현상태라고 보장하기어려워 보다 유저의 경험이 좋았으면 하는 바람에 사용하였습니다. (덤으로 기본디자인이 너무 맘에들어 실제 관리자페이지 프로젝트에도 많이 애용하고 있습니다.)

### Supabase
Supabase는 postgreSQL을 기반으로 만든 firebase의 SQL버전입니다. 그냥 postgreSQL을 사용하면되는걸 supabase를 사용한 이유는 인증관리나 권환관리 혹은 외부 API의 Oauth인증로그인 등 많은 편리함을 제공해주고, 스토리지를 제공해줌으로써 이미지, 비디오, 문서와같은 파일들을 업로드 할 수 있게 도와줍니다. 

더 많은 장단점이 있겠지만 제가 택한이유는 위와 같습니다.

### prisma.io
prisma는 sql문을 보다 편하게 자바스크립트 언어로 다룰 수 있게 해주는 라이브러리입니다. 제가 프론트/백 둘다 자바스크립트 기반의 프레임워크들을 사용하기도 하고, sql을 드라마틱하게 다룰줄 모르기에 ORM중에서도 다양한 자동화기능을 많이 제공해주는 prisma를 택하게 되었습니다.

> ORMdms (Object-Relational Mapping)의 약자로 DB의 relation과 object를 맵핑해주는 기술로써 sql 쿼리문을 사용하지않고도 DB를 사용할 수 있게 도와주는 도구입니다.