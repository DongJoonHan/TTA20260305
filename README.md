# TTA20260305

# Openjdk 25 다운로드 위치

# SonarQube 다운로드 위치

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




