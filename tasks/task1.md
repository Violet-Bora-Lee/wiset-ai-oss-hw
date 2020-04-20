# 과제 1 (난이도 하)

![GitHub Triangle](../resources/git-and-github-initial-setup.png)

(그림 [출처](https://docs.microsoft.com/en-us/contribute/get-started-setup-local))

> 위 그림을 참고해 하단부의 빈칸을 완성해주세요. 들어갈 수 있는 단어 혹은 명령어는 다음과 같습니다.

- origin
- upstream
- 클론
- 포크
- merge
- fetch
- rebase
- git pull
- git clone
- git remote add upstream

 
## 로컬 머신에 작업 환경 구축하기

오픈소스 기여의 시작은 기여하고자 하는 리포지토리를 내 계정으로 포크하는 것부터 시작됩니다. 포크가 완료되면 내 GitHub 계정에서 포크한 리포지토리의 주소를 확인할 수 있습니다.

포크 받은 리포지토리 주소 앞에 git clone를 붙여 만든 명령어를 로컬 머신(내 컴퓨터)에 입력하면 로컬 머신에 해당 리포지토리를 클론받을 수 있습니다.

참고로, git clone 명령어로 리포지토리를 최초로 클론받는 경우, 해당 리포지토리의 기본 별명은 origin이 됩니다.

## 소스 코드 최신으로 유지하기

최신 소스 코드를 받아오려면 먼저, 최신 소스 코드가 담긴 리포지토리를 내 로컬 환경과 연결해줘야 합니다. 이럴 땐 git remote add upstream이라는 명령어를 사용하면 됩니다.

upstream은 origin과 같이 리모트 리포지토리를 식별할 수 있는 별명으로, 이름표와 같기 때문에 원하는 대로 수정할 수 있습니다. 다만, 대부분의 git·GitHub 튜토리얼에서 포크 받은 리포지토리는 origin, 원 리포지토리는 upstream이라는 별명을 붙여 식별하기 때문에 이런 식별 방법을 미리 알아두는 것이 좋습니다.

upstream 리포지토리에 있는 최신 변경분을 로컬 리포지토리에 가져오는 방법은 다양합니다. 가장 쉬운 방법은 git pull명령어를 사용하는 것입니다. pull은 fetch와 merge를 합한 명령어입니다.

이외에도 fetch 후, rebase를 사용하는 방법이 있는데, rebase는 브랜치를 깔끔하게 관리할 수 있다는 장점이 있습니다. 다만, rebase를 사용하면 커밋 식별자가 변경되기 때문에, 이 점에 주의해야 합니다.
