# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## 프로젝트 개요

HTML, CSS, JavaScript(Vanilla), Tailwind CSS로 제작하는 반응형 1페이지 개발자 웹 이력서 프로젝트입니다. 상세 작업 계획은 `roadmap.md`를 참고하세요 (프로젝트 설정 → 이력서 콘텐츠 정의 → HTML 마크업 → Tailwind 스타일링 → JS 인터랙션 → 최적화/배포 순).

현재 저장소에는 아직 소스 코드가 없으며 `roadmap.md`만 존재합니다. Tailwind CSS 적용 방식(CDN 방식 vs CLI 빌드 방식)은 아직 확정되지 않았으므로, 실제 빌드/린트/테스트 명령어는 해당 도구가 설치된 이후 이 문서에 추가해야 합니다.

## 언어 및 커뮤니케이션 규칙

- 기본 응답 언어: 한국어
- 코드 주석: 한국어
- 커밋 메시지: 한국어
- 문서화(README, roadmap 등): 한국어
- 변수명/함수명: 영어 (코드 표준 준수)

## 아키텍처 방향

- 단일 페이지(1-page) 구조로, 시맨틱 HTML 태그(`header`, `nav`, `section`, `footer`)로 섹션을 구성합니다.
- 스타일은 Tailwind CSS 유틸리티 클래스를 우선 사용하고, `tailwind.config.js`로 색상/폰트 등 테마를 커스터마이징합니다.
- 인터랙션(스무스 스크롤, 다크모드 토글, 모바일 메뉴 등)은 별도 프레임워크 없이 Vanilla JavaScript로 구현합니다.
- 반응형 브레이크포인트는 Tailwind의 `sm:`, `md:`, `lg:` 접두사를 기준으로 설계합니다.
