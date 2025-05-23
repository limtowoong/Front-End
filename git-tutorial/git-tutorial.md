# Git & GitHub 입문 가이드

이 가이드는 Git과 GitHub를 처음 사용하는 입문자를 위한 실습 중심의 단계별 가이드입니다. 꼭 필요한 작업만 간결하게 설명합니다.

---

# 1. Git과 GitHub 연결하기

## 1.1 Git 설치 확인
```bash
git --version
```

## 1.2 GitHub 계정 생성
- [https://github.com](https://github.com) 에서 계정을 생성합니다.

## 1.3 Git 사용자 정보 설정
```bash
git config --global user.name "Your Name"
git config --global user.email "youremail@example.com"
```

## 1.4 SSH 키 생성 및 GitHub에 등록
```bash
ssh-keygen -t ed25519 -C "youremail@example.com"
```

> 키를 GitHub에 등록: GitHub > Settings > SSH and GPG keys > New SSH Key

---

# 2. 로컬 저장소 만들기

## 2.1 작업 폴더 생성
```bash
mkdir my-first-repo
cd my-first-repo
```

## 2.2 Git 초기화
```bash
git init
```

## 2.3 README.md 파일 만들기
```bash
echo "# My First Repository" > README.md
```

---

# 3. GitHub 원격 저장소 만들기

## 3.1 GitHub에서 새 저장소 생성
- GitHub 웹사이트에서 `New repository` 클릭 후 저장소 이름을 입력합니다.

## 3.2 원격 저장소 연결
```bash
git remote add origin git@github.com:yourusername/repo-name.git
```

---

# 4. 변경사항 커밋하고 푸시하기

## 4.1 변경된 파일 확인
```bash
git status
```

## 4.2 파일 스테이징
```bash
git add .
```

## 4.3 커밋 생성
```bash
git commit -m "Initial commit"
```

## 4.4 GitHub에 푸시
```bash
git push -u origin main
```

---

# 5. 이후 작업 흐름

## 5.1 파일 수정 후 커밋
```bash
git add .
git commit -m "작업 내용 작성"
```

## 5.2 GitHub에 다시 푸시
```bash
git push
```

---

> 🎉 축하합니다! 이제 Git과 GitHub의 기본적인 흐름을 익혔습니다. 자주 연습해보며 익숙해지세요.
