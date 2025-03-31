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
