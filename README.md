# 국립국어원 표준국어대사전 표제어 DB

## 개요

[2018 DMZ 해커톤](https://dmzhackathon.org/dmz-hackathon-2018)에서 [**남한말 vs 북한말 끝말잇기 게임**](https://github.com/korean-word-game) 을 개발하기 위해 만들어진 DB입니다.
2018.11.13 에 국립국어원 표준국어대사전을(http://stdweb2.korean.go.kr) 발췌하여 DB를 구축하였으며 오픈소스의 발전과 우리말 연구를 위한 다양한 분들에게 도움이 되었으면 하는 마음으로 이를 공유합니다.

## 저작권

본래 [저작권법 제24조의2](http://www.law.go.kr/%EB%B2%95%EB%A0%B9/%EC%A0%80%EC%9E%91%EA%B6%8C%EB%B2%95/%EC%A0%9C24%EC%A1%B0%EC%9D%982)에 의하면 국가에 의해 작성되어 공표된 저작물은 허락없이 이용할 수 있어야 하지만, 표준국어대사전의 경우에는 국립국어원이 저작재산권의 전부를 보유하고 있지 않으므로 저작권 등록물에 해당됩니다. 그러나 단순히 낱말과 품사를 수집한 것은 한국어 자체로써 저작권 보호를 받을 수 없는 자료이므로 자유로운 수정과 배포가 가능합니다.

## 크롤러
https://github.com/korean-word-game/crawling 에서 크롤링에 쓰인 소스를 공개합니다.

## 다운로드 (From GoogleDrive)

### ko-KR



#### [kr_korean.csv](https://drive.google.com/open?id=1PdzYubqcPKAIsHRtWZEFdQ1m4-fba6Oj) (9.72MB)

| 첫번째 열 | 두번째 열 |
| -------- | --------- |
| 낱말     | 품사      |



#### [kr_korean.db](https://drive.google.com/open?id=1mb9qpk4yRvkMICQ9bO21ocI1S7B2tWD4) (13.5MB)
```
# SQLite format 3
kr (TABLE)
┣━━━ id   (INTEGER)
┣━━━ word (TEXT)
┗━━━ part (TEXT)
```



#### [korean_kr.sql](https://drive.google.com/open?id=1fQqX_AYc1Mo_oaVHtIDnXDRhjI2Plk97) (17.8MB)
```
# 5.7.24 - MySQL Community Server (GPL)
-- --------------------------------------------------------
-- SQL 내보내기 설정
-- 데이터베이스:     생성
-- 테이블:           생성
-- 데이터:           삽입 무시 (기존 데이터를 갱신하지 않음)
-- 최대 INSERT 크기: 1024 KB
-- --------------------------------------------------------

korean (DB)
┗━━ kr (TABLE)
    ┣━━ id   (INT)
    ┣━━ word (TEXT)
    ┗━━ part (TEXT)
```

### ko-KP

#### [kp_korean.csv](https://drive.google.com/open?id=1OC7CYnEVV_PMmYJHlvfChFvdyLZbZ3zr) (1.32MB)

| 첫번째 열 | 두번째 열 |
| -------- | --------- |
| 낱말     | 품사      |



#### [kp_korean.db](https://drive.google.com/open?id=1H6Fb8frFvOC2-96prcFoAi3dZWJstOoD) (1.80MB)
```
# SQLite format 3
kp (TABLE)
┣━━━ id   (INTEGER)
┣━━━ word (TEXT)
┗━━━ part (TEXT)
```



#### [korean_kp.sql](https://drive.google.com/open?id=1AF1VimW41GhPn5jDEBdkk2SAaAufultt) (2.31MB)
```
# 5.7.24 - MySQL Community Server (GPL)
-- --------------------------------------------------------
-- SQL 내보내기 설정
-- 데이터베이스:     생성
-- 테이블:           생성
-- 데이터:           삽입 무시 (기존 데이터를 갱신하지 않음)
-- 최대 INSERT 크기: 1024 KB
-- --------------------------------------------------------

korean (DB)
┗━━ kp (TABLE)
    ┣━━ id   (INT)
    ┣━━ word (TEXT)
    ┗━━ part (TEXT)
```

### ko-KR & ko-KP

#### [kr_kp_korean.db](https://drive.google.com/open?id=1AQ3wwMGTmhR32p3k9V_RNw1JME__MaHM) (15.3MB)
```
# SQLite format 3
kr (TABLE)
┣━━━ id   (INTEGER)
┣━━━ word (TEXT)
┗━━━ part (TEXT)

kp (TABLE)
┣━━━ id   (INTEGER)
┣━━━ word (TEXT)
┗━━━ part (TEXT)
```



#### [korean_kr_kp.sql](https://drive.google.com/open?id=1e4JMfAub-VKXx4vKMcDMzqbdUL8gdHeC) (20.1MB)
```
# 5.7.24 - MySQL Community Server (GPL)
-- --------------------------------------------------------
-- SQL 내보내기 설정
-- 데이터베이스:     생성
-- 테이블:           생성
-- 데이터:           삽입 무시 (기존 데이터를 갱신하지 않음)
-- 최대 INSERT 크기: 1024 KB
-- --------------------------------------------------------

korean (DB)
┣━━ kr (TABLE)
┃   ┣━━ id   (INT)
┃   ┣━━ word (TEXT)
┃   ┗━━ part (TEXT)
┃
┗━━ kp (TABLE)
    ┣━━ id   (INT)
    ┣━━ word (TEXT)
    ┗━━ part (TEXT)
```

