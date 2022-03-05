# web1
생활코딩-html강의
using github, learning how to use free web server hosting.


git에 대해 알게된점
 - 로컬저장소 사용자정보
    로컬저장소에 처음 글로벌로 저장한 user.name과 user.email은 깃허브 username과 useremail와 연관되어 있다.
    로컬에서 커밋할때 name이 같아도 다른 유저[예를 들어 내 다른 아이디 errorfixie]와 연동된 email이라면 다른 유저의 이름으로 커밋될 수 있다.
    이번 경우에선 umcondo로 커밋하려했는데, 로컬 useremail이 errorfixie와 연동되어 있어 errorfixie로 커밋되었다.
    git config user.name, git config user.email로 기존 사용자정보를 알 수 있었다.
    git config user.name [새이름], git config user.email [새이메일]로 정보를 바꿀 수 있었다.

 - 커밋 되돌리는 방법 2가지
    이와 관련하여 원격저장소(깃허브)에 커밋된 내용을 되돌리려고 하였다.
    로컬에서 git reset --hard [돌아가고싶은커밋번호]를 하여 커밋을 되돌린 후
    git push -f origin을 해서 원격저장소까지 되돌릴 수 있었다.

    커밋내역까지 모두 없어져서 errorfixie로 커밋한 내역이 모두 사라졌다.
    다른 아이디로 커밋한 내역을 없앨때는 이런 방법이 맞지만
    다른 사람과 같이 쓰거나 커밋한 내역과 지운 내역을 모두 남기고 싶다면 git revert를 이용해야 한다고 한다.

    참고한 블로그 : [https://jupiny.com/2019/03/19/revert-commits-in-remote-repository/](https://jupiny.com/2019/03/19/revert-commits-in-remote-repository/)
    