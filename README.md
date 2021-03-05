## Git 생성& 커밋& 푸시 커맨드
```
git init
```
 현재 디렉토리에 깃을 이니시함
 
___

```
git remote add **origin** _https://~~~.git_
```
 내가 이니시한 그 디렉토리 의 깃을 깃허브의(remote)저장소와 연결.
 
 ___
```
git remote -v
```
 깃허브(remote)저장소와 연결이 됬는지 확인하는 커맨드.
 잘 되었다면 메세지가 아래와같이 뜬다.

>**origin** _https://~~~.git_ (fetch)
>**origin** _https://~~~.git_ (push)

___
```
git add * 
```
 변경사항을 git 에 staging.
git commit -m"첫커밋"
 staging된 변경사항을 코멘트 달아서 커밋.
 
___
```
git push **origin** _master_
```
 푸시 커맨드. 아직 아무것도 푸시 되지 않아서,master이라는 브랜치가 만들어 지면서 푸시된다.
 
___
___
___


## Git 브랜칭
```
git branch
```
 현재 생성되어있는 브랜치들 목록과, 현재 어떤 브랜치에서 작업중인지 보여준다. 이 상태에서 다시 쉘로 나가려면, q 를 누른다.
 처음 푸시를 했으면 그때 푸시한 이름으로 만들어진 브랜치밖에없다.(주로 main 이나 master 로 이름 짓는것같다.)
 

___

```
git branch _feature/readme_
```
 feature/readme 이라는 브랜치가 새로 만들어진다.
 
```
git checkout _feature/readme_
```
 그 브랜치에서 작업하기로 변경한다.
![](https://images.velog.io/images/coldfeet0816/post/2e718552-3f7b-418a-bd99-630b152b539f/image.png)

이상태에서 다시 git branch를 한다면, 새로운 브랜치가 생성되있는 것을 확인할 수 있다.

___
