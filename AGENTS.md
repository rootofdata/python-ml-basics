# AGENTS.md

Python·pandas·scikit-learn 기초 학습 노트북 모음(3개 저장소 통합본). 범용 코딩 에이전트를 위한 안내 문서.

## 명령어

- 설치: `pip install numpy pandas matplotlib seaborn scikit-learn jupyter`
- 실행(.ipynb): Jupyter 또는 VS Code에서 셀 실행
- 실행(.py): `python <파일>` (예: `python-basics/ipython_bug.py`)
- 테스트: 별도 프레임워크 없음
- 데이터: 타이타닉 CSV는 `data/`에 위치

## 구조

- `python-basics/` — Python 기초 문법·예제
- `pandas-numpy/` — numpy/pandas 및 교재 챕터(Chapter6~14)
- `sklearn-ml/` — 전처리·교차검증·타이타닉 예측·평가지표
- `bootcamp/` — 부트캠프(데청캠) 실습
- `data/` — 타이타닉 실습 데이터

## 컨벤션

- 이름이 같고 내용이 다른 파일은 원본 저장소명을 접두어로 붙여 구분(이 규칙 유지)
- 파일명에 한글·공백·번호 혼용. 기존 방식 존중
- 기본 브랜치는 `master`

## 주의

- 일부 노트북은 데이터를 옛 로컬 절대경로(OneDrive 등)로 읽는다. 실행 시 `data/` 기준 상대경로로 조정하되 대량 일괄 수정은 지양
- `data/`의 CSV 등 대용량 데이터 삭제 금지
- 파일 이동 시 노트북 내부 상대경로 참조 깨짐 주의
- 한글 파일명 NFC 통일, `.ipynb_checkpoints/`·`__pycache__/`·`.DS_Store` 커밋 금지
- CLAUDE.md와 내용 동일하게 유지
