# linux-commands-assignment
20253008 최태민 오픈소스SW개론 과제2

# 1) 작업 디렉토리 만들기
mkdir ~/linux-commands-assignment
cd ~/linux-commands-assignment

# 2) README.md 파일 생성 (에디터로 열어 위에서 준 템플릿 붙여넣기)
# 예: nano, vim, code 등
nano README.md
# (내용 붙여넣고 저장)

# 3) 이미지 폴더 만들기 (스크린샷 넣을 때)
mkdir -p images

# 4) git 초기화 및 원격 연결
git init
git add README.md
git commit -m "Add README for assignment"

# 아래 URL은 네가 만든 리포지토리 주소로 바꿔써야 함
git remote add origin https://github.com/<your-username>/linux-commands-assignment.git
git branch -M main
git push -u origin main
