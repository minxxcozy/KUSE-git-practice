## 🎯 시험 목적
본 시험은 **로컬 작업 → 브랜치 → 커밋 → 원격 푸시 → PR 생성**까지
전체 실무 워크플로우를 **정확히 수행할 수 있는지**를 평가합니다.

## 📦 제공 사항
* GitHub 원격 저장소 (사전 제공)
* 해당 저장소는 clone 권한만 있습니다.
* 모든 작업은 **Fork → Pull Request(PR) 방식**으로 진행합니다.

## 📝 실습 과제
### 1️⃣ 저장소 Fork & Clone
1. 시험용 GitHub 레포지토리를 본인 계정으로 Fork
2. Fork한 저장소를 로컬로 clone

### 2️⃣ 새 작업 브랜치 생성
> ⚠️ main 브랜치에서 직접 작업 ❌

브랜치 이름 규칙은 아래와 같습니다.
```bash
feat/add-kuse-<english-name>
```

예시 : 
```bash
feat/add-kuse-minchae
```

### 3️⃣ 디렉토리 및 파일 생성
**📁 디렉토리 구조**
* 프로젝트 루트에 **본인 이름으로 된 폴더 생성**
* 해당 폴더 아래에 Python 파일 1개 생성

예시는 다음과 같습니다.
```markdown
kuse-git-practice/
 └── minchae/
     └── minchae.py
```

### 4️⃣ Python 파일 내용 작성
**📌 요구 사항**
* 반복문을 사용하여 1부터 5까지의 숫자를 한 줄씩 출력하는 Python 코드를 작성하세요.

**📤 출력 예시**
```bash
1
2
3
4
5
```

### 5️⃣ 커밋 생성
* 변경 사항 스테이징 후 커밋
* 커밋 메시지 예시 :
```
feat: add python file
```

### 6️⃣ 원격 저장소(origin)로 push
* 생성한 브랜치를 origin(내 fork) 으로 push

### 7️⃣ Pull Request 생성
* GitHub 웹에서 Pull Request 생성
* PR 방향 :
```
내 fork (origin) → 원본 저장소 (upstream/main)
```
* PR 제목 :
```
KUSE 7기 4주 차 "본인이름"
ex. KUSE 7기 4주 차 김민채
```

## 🔎 (참고) origin / upstream
### ✔️ 현재 원격 저장소 확인
```bash
git remote -v
```

### ✔️ (선택) upstream 등록
```bash
git remote add upstream https://github.com/원본조직/kuse-git-practice.git
```
