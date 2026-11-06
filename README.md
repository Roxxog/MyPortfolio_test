# 필요한 도구 버전

Hugo v0.146.2 이상 (이 사이트는 Hugo v0.167.0 사용 중)

Go (버전 : go version go1.27.3 windows/amd64)

Beautiful Hugo themes v5.0.0 (https://github.com/halogenica/beautifulhugo 공식 github 저장소에서 다운로드)

Python 3.15.2 사용 (Python 3.9 이상)

git 2.50.1.windows.1 사용됨

# 실행 절차 (git 폴더 생성, 저장소 생성, 빌드 확인 절차)

다운로드한 휴고 테마 압축해제 후 beautifulhugo-master폴더를 git이 관리하게 될 폴더에 넣은 후 prepare_github_pages.py를 추가로 넣어준다.

github에서 저장소를 생성한 후 저장소의 HTTPS 주소를 복사한다.

PowerShell 등의 터미널에서 cd를 통해 휴고 테마 폴더로 이동한다. (ls를 통해 README.md, layouts 등의 파일과 함께 prepare_github_pages.py가 있는 것을 확인)

python prepare_github_pages.py 명령어를 실행한 후 저장소의 HTTPS 주소를 붙여넣어은 후 이어서 명령어를 실행한다. (만약 명령어 실행 환경이 bash 등일 경우 작동하지 않을 수도 있음)

명령어가 정상적으로 실행되었을 경우 저장소로 이동하여 Settings -> Pages -> Build and deployment 설정을 Github Actions로 변경한다.

휴고 테마 폴더를 git init . 그리고 git remote add origin 저장소의 HTTPS 주소 명령어를 이용하여 Github 저장소와 연결시켜준다. (git remote -v 명령어로 github 주소가 나올 경우 잘 실행되었다고 할 수 있다)

git branch -M main 으로 브랜치를 main으로 설정해준다. (간혹 main이 아닌 master로 브랜치가 설정되어 있을 수 있기 때문에 로컬의 브랜치 이름과 저장소의 브랜치 이름을 통일 시켜 혼란을 없앤다)

git add . -> git commit -m "원하는 초기 커밋 메세지" -> git push origin main 순으로 명령어를 입력하여 로컬 폴더의 상태를 저장소에 저장한다. (그리고 Actions에서 배포된 주소로 들어가 배포된 사이트를 확인한다)

prepare_github_pages.py 로 생성된 site/content, site/hugo.toml 등의 파일들을 수정하며 사이트를 개선한다.

winget install -e --id Hugo.Hugo.Extended 명령어를 실행하여 Hugo를 다운받아서 사이트를 미리보기 할 수 있다. 

hugo server --source site 명령어로 나온 local 주소를 통해 사이트를 미리 볼 수 있다. (만약 Go와 관련된 Error가 발생할 경우 아래에서...)

winget install -e --id GoLang.Go 명령어는 만약 beautifulhugo-master/site 기준으로 배포된 사이트를 미리 보기할 때 Go 프로그래밍 언어가 설치가 안되어있을 경우 Error가 발생할 때 Go를 다운받은 후 다시 hugo server --source site 명령어를 실행하여 local 주소를 통해 사이트를 미리보기 한다.(local 주소의 사이트는 미리보기 용으로 해당 local 주소는 배포용 주소가 아니다)

# 수정과 재배포

배포되는 사이트는 beautifulhugo-master/site의 폴더를 수정하여 변경할 수 있다.

파일들을 수정한 후 PowerShell에서 cd를 통해 beautifulhugo-master로 이동한 후 git add . -> git commit -m "커밋 메세지" -> git push origin main을 통해 저장소에 commit을 남기면 배포가 자동으로 일어나며 Actions에서 배포의 성공 여부를 확인할 수 있다.

배포가 성공할 경우 공개 사이트 주소를 통해 사이트를 확인한다.