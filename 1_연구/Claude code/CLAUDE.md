# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## 연구 개요

석사 1학기 연구 과제: **무인기용 터보프롭 엔진의 디지털 트윈 구축 및 AI 기반 상태기반정비(AI-CBM+)**

- 엔진 모델: Garrett TPE331 계열 터보프롭 엔진
- 도구: Ansys Twin Builder (디지털 트윈), Python (데이터 분석)
- 목표: 엔진 상태 모니터링 → 이상 탐지 → 정비 예측

## 폴더 구조

```
1_연구/
├── Claude code/        # Claude Code 보조 작업 (현재 위치)
│   └── 엔진 분석/      # 엔진 데이터 분석 스크립트
├── KSAA/               # 한국항공우주학회 학술대회 자료
├── Twin Builder/       # Ansys Twin Builder 가이드
├── 엔진/               # TPE331 엔진 참고문헌 및 제원
│   ├── TPE331 제원/    # 정비 매뉴얼, TCDS, Training Manual
│   └── 군용엔진관품질인증관련문서모음압축/  # JSSG, MIL 규격
└── 제안서/             # 연구 제안서
```

## 주요 참고 자료 위치

- TPE331 정비 매뉴얼: `1_연구/엔진/TPE331 제원/692982076-Garrett-TPE-331-10-Maintenance-Manual.pdf` (100MB 초과, GitHub 미업로드)
- CBM 관련 논문: `1_연구/엔진/Aero engine heath monitoring, diagnostics and prognostics for condition-based maintenance an overview.pdf`
- 엔진 모델링 대화 기록: `1_연구/엔진/[최종 통합본] 항공기 추진 및 터보프롭 동적 시스템 모델링 전체 대화 기록.docx`
- 주요 파라미터: `1_연구/주요 파라미터.xlsx`

## GitHub 자동 동기화

이 디렉토리(`MYBOX-asdf101000/개인 폴더/2026`)는 **5분마다 자동으로 GitHub(`chestnutbread/2026-1`)에 push**됩니다.
- 동기화 스크립트: `~/sync-2026.sh`
- 로그: `~/.sync-2026.log`
- 100MB 초과 파일 및 `*편집충돌*` 파일은 `.gitignore`로 제외됨

## 응답 지침

- **언어**: 별도 요청이 없으면 항상 한국어로 답변
- **전문 용어**: 전문 용어 사용 시 괄호 안에 쉬운 말로 풀어서 함께 설명
- **결과물 저장**: 작업 결과는 항상 파일로 저장. 저장명 형식: `파일명_YYYYMMDD` (예: `분석결과_20260509`)
- **작업 전 확인**: 작업 시작 전 수행할 내용을 먼저 설명하고, 사용자 확인 후 진행
- **질문 검토**: 사용자의 질문에 오류나 전제 오류가 있을 경우 먼저 정정한 뒤 답변
- **추가 질문 선 제시**: 답변 후 사용자가 이어서 물어볼 만한 추가 질문 2~3가지를 먼저 제시
- **핵심 포인트 강조**: 설명 시 중요한 부분과 초보자가 헷갈리기 쉬운 포인트를 명시적으로 구분하여 제시
- **핵심 요약**: 모든 답변 마지막에 핵심 3줄 요약 포함
- **출처 명시**: 정보 제공 시 해당 출처(논문, 매뉴얼, 문서 경로 등)를 함께 제시
- **복붙용 문서 작성**: 복사·붙여넣기용 문서 요청 시, 기계적 표현을 제거하고 사람이 쓴 것처럼 자연스럽되 공식적이고 신뢰감 있는 톤으로 작성

## 도메인 용어

- **CBM** (Condition-Based Maintenance): 상태기반정비
- **PHM** (Prognostics and Health Management): 예지보전
- **Digital Twin**: 물리 엔진의 실시간 가상 복제본
- **TPE331**: Garrett(현 Honeywell) 제조 터보프롭 엔진
- **JSSG-2007A/2008**: 미 국방부 엔진 개발 규격
