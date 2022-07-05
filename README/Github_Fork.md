### 깃허브 협업

1.	레포지터리 생성 -> 팀장
2.	상단 Fork 생성 -> 팀원 깃허브에 생성
3.	코드 https 주소 복사 -> 나의 깃허브 주소
4.	Gitbash 터미널 열기
5.	git clone ‘내 레포지터리 https 주소’
![](https://velog.velcdn.com/images/zakumann/post/5c902faa-5a2c-4028-a7b5-f5b94fa40d90/image.png)

6.	경로 확인, 경로 이동은 cd ‘폴더 이름’
git remote add upstream ‘팀장 레포지터리 https 주소’
![](https://velog.velcdn.com/images/zakumann/post/21c6e98e-7f62-4002-b825-dcc3d1de2756/image.png)

7.	연결 확인
git remote -v
![](https://velog.velcdn.com/images/zakumann/post/3c9b1a63-b947-471c-a05f-701ce140ac01/image.png)


8.	전체 파일 add: git add . 
커밋 작성: git commit -m ‘커밋내용’
![](https://velog.velcdn.com/images/zakumann/post/16c2fcc7-3567-43bd-99c0-7a626bc0dbf8/image.png)


9.	내 레포지터리에 전송
git push
![](https://velog.velcdn.com/images/zakumann/post/2363bd10-3f5c-4919-a0a8-c6e1e073de07/image.png)


10.	내 레포지터리 깃허브에 링크 활성화되어 있음 확인 > 링크 클릭 후 업로드 버튼 클릭
'팀장이 pull 확인하고 merge 승인 후'
![](https://velog.velcdn.com/images/zakumann/post/7dd2d438-8699-4fcd-bfe6-16b3fdc43c90/image.png)

11.	(팀장 저장소와 내 저장소 일치화 과정)패치
git fetch upstream
![](https://velog.velcdn.com/images/zakumann/post/b4fde0c1-4d50-46a1-b855-e238124dfaf7/image.png)




12.	저장소에 차이점을 찾아 변경사항 적용
git merge upstream/main
(내 작업 VS에 없고 팀장 레포지터리에 있던 작업파일 생성됨)
![](https://velog.velcdn.com/images/zakumann/post/1c52f7fd-3a78-44dd-9167-ee77114620b9/image.png)


 
13.	다시 내 저장소에 push
git push
![](https://velog.velcdn.com/images/zakumann/post/2e2ed444-7db4-4ef0-b8cc-0c1a9db9e911/image.png)


### 깃허브 Fork

fork는 개발자들끼리 협업을 할때 쓰인다.
여기서 오해하지 말아야할 것이, 협업을 할때 쓰인다는게, 자기 팀끼리의 협업을 말하는게 아니다.
 
간단히 설명하자면, 원작자의 코드를 fork 하면, 자신의 원격 저장소에서 코드를 마음대로 뜯어 고칠 수 있다.
[코드짜는 문과녀:티스토리](출처: https://eunhee-programming.tistory.com/159)