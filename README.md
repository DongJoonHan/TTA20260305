# 2026 SonarQube 교육


# Junit4 프로젝트 파일 위치
https://github.com/DongJoonHan/junit4

## Git으로 클론 받는 방법
```
git clone https://github.com/DongJoonHan/junit4.git
```

# Docker 실행
## Docker Desktop 다운로드 위치
https://docs.docker.com/desktop/setup/install/windows-install/

## Docker Hub 공식 사이트
https://hub.docker.com/_/sonarqube

## Docker compose file 위치
https://github.com/SonarSource/docker-sonarqube/blob/master/example-compose-files/sq-with-postgres/docker-compose.yml
(우상단 다운로드 버튼으로 다운로드함)

# Sonar-Scanner in Docker
Docker에서 Sonar-Scanner로 실행할 때, 
Mount 된 Host의 Workspace에 압축을 해제하고,
각 Job에서 상대 경로로 접근

## 폴더 구성
<img width="472" height="94" alt="image" src="https://github.com/user-attachments/assets/411344b7-1ff9-439c-894d-7374dcbf6585" />

## Job에서 Execute Shell 로 실행
```
../sonar-scanner-linux/bin/sonar-scanner \
  -Dsonar.projectKey=Design_jenkins \
  -Dsonar.sources=. \
  -Dsonar.host.url=http://IP:9000 \
  -Dsonar.token=sqa_token값
```

# 몇 가지 분석 팁
## Git 등의 변경 이력을 추적하지 않는 경우
- 보통 다운로드 받은 코드를 분석하는 경우
<img width="2000" height="971" alt="image" src="https://github.com/user-attachments/assets/d581d1cb-21d4-40bf-b71f-f4ce77eb9087" />

## 순환복잡도 룰 추가
<img width="2000" height="861" alt="image" src="https://github.com/user-attachments/assets/ad979ed3-3783-4a80-962a-4fd2545f5c28" />

# Sonarqube 대안
## 룰 기반 정적분석
- Java: PMD, FindBug
- C/CPP: CppCheck
- python: pylint / pycodestyle

## (함수별) 순환 복잡도 / 라인수
- Lizard (Python 패키지) : 언어 안따짐

## 전체 라인수/주석비율
- CLOC : 언어 안따짐

## 복사/붙여넣기 코드
- PMD -> CPD: PMD 6.55.0 언어 안따짐

## 코딩 스타일(컨벤션)
- 구글 표준 https://google.github.io/styleguide/
- cpplint 도구로 확인 가능

## 위 도구 사용 방법 링크
https://github.com/DongJoonHan/QAInfo




