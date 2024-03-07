# 프로젝트명

- 심청이(SimcheongE)
  - 심플한 청년의 이익
  - Simple Cheongnyeon Economy
  - 청년들에게 필요한 정책들을 간단하게 제공하는 서비스

# 주제 (청년 금융 지원 정책 플랫폼)

- 도메인 : 핀테크
- 청년들을 위한 청년 정책 정보 제공

# 서비스 대상

- 만 19 ~ 34세 청년(향후 39세로 연장 될 수도 있다.)
- 자신이 참여할 수 있는 지원 정책 정보를 알고 싶은 청년
- 진행 중인 정책에 관심이 없거나 이해하지 못해 혜택을 놓치는 청년

# 서비스 목적

- 지역별로 제공되는 다양한 정책을 사용자가 선택하여 찾을 수 있게 제공.
- 나눠져 있는 각 지원 정책을 한 앱에서 확인
- 지원 정책과 청년에게 필요한 정보들을 제공 (지원 정책 및 정보 제공)
- 최대한 ‘간편하게’ 사용자에게 맞는 청년 정책 정보 제공 (편의성 향상)
- 재테크를 준비함에 있어서 기본적인 경제 및 사회 관련 용어 / 개념을 제공
  (경제 및 사회 개념 교육)
- STT 기반의 챗봇기능을 메인으로 구현하여, 접근성을 향상 (접근성 향상)

# 문제 인식

- **정책 다양성과 지역별 차이**: 청년을 대상으로 하는 다양한 정책들이 있으나, 지역마다 제공하는 정책에 차이가 있다.
- **정보와 서류의 복잡성**: 정책을 신청하기 위해 필요한 정보와 서류가 과도하게 많아, 신청 과정이 복잡하다.
- **서류 발급의 어려움**: 필요한 서류마다 발급 방법이 다르다.
- **신청 방법의 혼란**: 일부 서비스는 온라인으로만 신청 가능하거나, 반대로 오프라인으로만 신청을 받아 불필요하게 오프라인 방문을 하거나, 신청 기한을 놓치는 경우가 있다.
- **정책 정보에 대한 접근성**: 우리나라에 청년을 위한 많은 정책과 혜택들이 있지만 현실적으로 대다수의 청년들이 그 정보를 몰라서 정책을 이용하지 못하는 경우가 상당히 많다.

# 관련 정보

- https://www.c1news.kr/news/articleView.html?idxno=14179
- https://www.nypi.re.kr/brdrr/boardrrView.do?menu_nix=4o9771b7&brd_id=BDIDX_PJk7xvf7L096m1g7Phd3YC&cont_idx=798&seltab_idx=0&edomweivgp=R
- https://www.donga.com/news/Society/article/all/20190917/97433123/1

# 서비스 개요(메인 서비스)

- 서비스 실행 시 첫 화면에서 AI 챗봇 기능으로 시작
  - STT를 사용하거나, 직접 입력을 해서 필요한 서비스로 접근 가능
  - 챗봇을 사용하기 싫다면 버튼을 통해 바로 서비스로 접근 가능
- 사용자가 가입 시 입력한 정보를 바탕으로 자동 사용자 맞춤 정책 추천
- 사용자가 입력한 조건에 따라 관련 정책 추천
- 지역별 / 연령별 시행 중인 정책 정보 제공
- 게시판(공지사항 및 취업, 공모전 등의 Job Fair 자료 공유)
- 북마크 기능(로그인)
  - 사용자가 북마크 체크한 기사, 정책, 게시판 등을 한번에 볼 수 있는 기능 제공
- 설정
  - 사용자 정보 수정
  - 앱 설정

# **서브 기능**

- 챗봇(AI) - 파인튜닝
  - ~~용도에 따라 심리 상담 /~~ 정보 검색으로 나눔
- 현재 가장 인기 많은 정책, 이 정책에 관심이 많은 연령대, 성별 등의 통계 제공(API)
- 정책 신청 자격 요건(전처리)
  - 사용자의 상황을 분석하여 신청했을 때 승인/불가를 미리 검사해주는 시스템(모의 계산)
  - 단순 참고용임을 고지할 것
  - 굳이 한다면 WebView로 해당 사이트 보여주기
  - 중복 지원 확인
- 뉴스 요약(크롤링+AI)
- 정책 관련 기사들을 요약하여 제공
- ~~푸시 기능(실시간)~~
  - ~~북마크한 정책 중 서류 제출 기간이 다 되어가는 정책이 있을 때 푸시알림~~
- 정책 후기(커뮤니티)
  - 자신이 참여한 정책에 대해 후기를 남길 수 있는 게시판 제공
  - 정책 디테일 페이지에 들어갔을 때, 실제로 그 정책에 참여한 사람들이 그 정책에 대한 디테일한 정보를 공유할 수 있도록 댓글이나 짧은 게시글 추가 작성할 수 있는 공간 제공
- 주식 / 부동산 관련 재테크 정보 제공
  - 주식 / 경제 관련 단어
  - 부동산 계약 시 확인 사항(서류 및 전세 사기 사례 및 예방 방법)

# 활용 API

- [한국고용정보원 청년정책 정보 API(종결)](https://www.data.go.kr/data/15088883/openapi.do)