# [12์ฃผ์ฐจ] calloc, realloc, file pointer


### ๐ key word: `calloc`,  `realloc` , `file stream`, `file pointer`, `fopen`, `fprintf`, `fscanf`

<br>  

## calloc  
- ๋์ ์ผ๋ก ๊ณต๊ฐ์ ํ ๋น ํ 0์ผ๋ก ์ด๊ธฐํ  
```c
int *p = 0;
p = (int*)calloc( 5, sizeof(int) );
```
<img src="https://user-images.githubusercontent.com/61939286/142659333-0cb348b2-79f8-41da-ae9e-f93b5ea32faa.png" width="70%" >

- ํ ๋น ๋ฐ์ง ์์ ๊ณต๊ฐ๋ ์ฃผ์๋ก ์ ๊ทผํด ๋ค์ฌ๋ค ๋ณผ ์ ์์  
<img src="https://user-images.githubusercontent.com/61939286/142659145-e75a2783-5f85-4f5f-bb64-6ed080271217.png" width="70%" >

<br>  

## realloc  
- malloc์ผ๋ก ํ ๋น ๋ฐ์ ๊ณต๊ฐ์ ์ฌ ํ ๋น (ํ์ฅ, ์ถ์)  
```c
int *p = 0;
p = (int*)malloc( sizeof(int) * 5 );
p = realloc( p, sizeof(int) * 7);
```
![image](https://user-images.githubusercontent.com/61939286/142659893-dfea6553-ce99-4831-9e74-a9920eb0676c.png)

<br>  


## ํ์ผ ์คํธ๋ฆผ  
<img src="https://user-images.githubusercontent.com/61939286/142660360-43fc442a-f6ea-48cb-8d43-5c4c3f38ca9f.png" width="50%" >  

- ๋ฉ๋ชจ์ฅ์ผ๋ก ์ด์ด์ ๋ณด์ด๋ฉด text file, ์๋๋ฉด binary file(์ด๋ฏธ์ง, ๋ฌธ์,..)  

<br>  

## ํ์ผ ํฌ์ธํฐ  
- OS์์ ์๋ ํ์ผ์ด ์ ์ฅ๋์ด์๋ ๊ตฌ์กฐ์ฒด์ ๋ํ ์ฃผ์๋ฅผ ๊ฐ์ง๊ณ  ์์  
<img src="https://user-images.githubusercontent.com/61939286/142661548-95152635-3cac-4e42-84da-3e96b1b21403.png" width="70%" >
<img src="https://user-images.githubusercontent.com/61939286/142661862-b5a5dc3d-c85e-47bd-b641-7e27516e351d.png" width="70%" >

- ์์  (fopen, fclose, fprintf)  
  <img src="https://user-images.githubusercontent.com/61939286/142665098-0406a1cc-7047-40a4-8fd6-564c91bf49ac.png" width="70%" >

- ์์  (fscanf)
  ![image](https://user-images.githubusercontent.com/61939286/142667290-dd3d47d3-72c9-4ce3-83ae-fa8d4d267189.png)

  

<br>  




