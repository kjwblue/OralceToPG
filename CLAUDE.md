# 프로젝트: OralceToPG

Oracle에서 PostgreSQL로 전환 시 참고할 매핑 레퍼런스 프로젝트

## 프로젝트 구조
- `input/` — 사용자가 제공하는 엑셀 파일 (Oracle↔PG 매핑 테이블, 공란 포함)
- `output/` — 공란이 채워진 완성된 엑셀 파일

## 작업 흐름
1. 사용자가 `input/`에 엑셀 파일 배치
2. 엑셀을 읽고 공란 채우기 (타입 매핑, 함수 매핑, DDL/DML 변환 등)
3. 완성된 파일을 `output/`에 저장

## 컨텍스트
- 대상: Oracle → PostgreSQL 전환 중인 Java 개발자
- 범위: 데이터 타입, DDL, DML, 내장 함수, PL/SQL→PL/pgSQL, 시스템 뷰/카탈로그
- 엑셀 처리: Python(openpyxl/pandas)을 유틸리티로 활용 가능

## 규칙
- input/output 외 별도 문서나 폴더를 만들지 않는다
- 결과는 반드시 `output/`에 저장하고, `input/` 파일은 절대 덮어쓰지 않는다
- 주석과 코드는 영어, 응답은 한국어로 작성한다
