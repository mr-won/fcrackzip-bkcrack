fcrackzip 칼리에 디폴트로 있다면서 왜 없냐?

 

우분투에 설치 가능하대서 깔았음

sudo apt-get install fcrackzip

 

fcrackzip

-b : brute force

-D : dictionary

-c : a 영소문자, A 영대문자, 1 숫자, ! 특수문자, : 는 뭐지

-l : length

 

영소문자, 영대문자, 숫자 8자리로 돌린다 하면

fcrackzip -b -c aA1 -l 8 test.zip 

 

1-5자리는 -l 1-5 하면 됨

 

8자리 했더니 아직도 aa 돌고 있음.. 

순서대로 도니까 오래 걸림

bkcrack 고놈도 해봐야겠다

https://github.com/kimci86/bkcrack

 

kali 에 cmake 깔고 하면 되는데

내 칼리 2022.3-amd64 버전

얘는 동일 파일 하나라도 있을 때 압축 패스워드 바꿀 수 있는건데

AdminFile_2.zip 은 패스워드 걸린 zip
 

-C 비번걸린zip -c 동일파일 -P 비번안걸린zip -p 동일파일 -e

-C 비번걸린zip -k 키값 -U 새로만들zip 변경할pw
