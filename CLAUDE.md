# 프로젝트

Python·pandas·scikit-learn 기초 학습 및 실습 노트북 모음 (3개 저장소 통합본).

## 환경·실행

- 언어: Python 3, 실습은 대부분 Jupyter 노트북(`.ipynb`)
- 주요 패키지: `numpy`, `pandas`, `matplotlib`, `seaborn`, `scikit-learn`
- 실행: Jupyter 또는 VS Code에서 노트북 셀 실행. `.py`(`ipython_bug.py` 등)는 `python <파일>`
- 실습 데이터: 타이타닉 CSV는 `data/`(`titanic_train.csv`, `titanic_test.csv`, `titanic_gender_submission.csv`)에 있음
- 별도 빌드/테스트 프레임워크 없음

## 폴더 구조

- `python-basics/` — Python 기초 문법(문자열·함수·기초 예제), 텍스트 실습 파일 포함
- `pandas-numpy/` — numpy/pandas 기초 및 교재 챕터 실습(`Chapter6`~`Chapter14`)
- `sklearn-ml/` — scikit-learn 분류·회귀: 전처리·교차검증·타이타닉 예측·정확도/F1 등 평가지표
- `bootcamp/` — 부트캠프(데청캠) 날짜별 실습
- `data/` — 타이타닉 실습 데이터

## 컨벤션

- 통합 저장소이므로, 이름은 같지만 내용이 다른 파일은 원본 저장소명을 접두어로 붙여 구분 (예: `muching-learning_ex_basic.ipynb`, `python-machine-learning-guide_1-3. 데이터 전처리.ipynb`). 이 접두어 규칙을 유지할 것
- 파일명에 한글·공백·번호(`1-3.`, `2_2.`) 혼용. 기존 명명 방식 존중
- 기본 브랜치는 `master`

## 주의

- 일부 노트북은 데이터를 저장소 상대경로가 아니라 옛 로컬 절대경로(예: `C:/Users/.../titanic_train.csv`, OneDrive 경로)로 읽는다. 실행 시 경로를 `data/` 기준 상대경로로 바꿔야 하며, 이런 절대경로가 남아있어도 임의로 대량 수정하지 말고 필요한 노트북만 조정할 것
- `data/`의 CSV 등 대용량 데이터 파일은 삭제하지 말 것 (실습 재현에 필요)
- 노트북/파일 이동 시 노트북 내부의 상대경로 데이터 참조가 깨질 수 있으니 함께 확인
- 한글 파일명은 NFC로 통일
- `.ipynb_checkpoints/`, `__pycache__/`, `.DS_Store` 커밋 금지
