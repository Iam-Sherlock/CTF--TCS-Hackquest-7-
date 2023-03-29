# CTF-writeups TCS hackquest Season 7
![1673355147517-nizenberg](https://user-images.githubusercontent.com/53529867/211574610-12fa243b-c526-412c-bacc-23f2d79ba81f.jpeg)
# Other than this there are two questions which has been changed during the Contest >>
## Solved Questions 
### 1) Rorchash Test (VS test)

In the Rorschach test the description was really big story it has quoted that a mathematician hidden the quote in a normal text. 
Then moved to the website and saw the word wazhuh! A n number of times where if you copy and paste in a text editor whole linux machine will hung and meanwhile the google docs went unresponsive after pasting so i did scrolled all the way from start to end then found some letters in between the words “wazhuh” and merged all the words got the flag

Flag: HQ7{f0u4$y}

### 2) Sassy Spaghetti
![1673362785758-very-nize](https://user-images.githubusercontent.com/53529867/211585619-a224ca23-83a2-47c6-842c-7578d578b4c2.png)

In the above image it redirects to the page where meme shows "LET ME IN" and then it shows you dont have administrator profile
then tried putting /robots.txt in URL there is a context with disallow "check.php.bak" 

![Screenshot from 2023-01-07 13-55-47](https://user-images.githubusercontent.com/53529867/211585995-620876b2-56b9-408f-89dc-1fc6f5c62dc3.png)

From the above image You can clearly see 2 memes and it also says about the administrator profiles
Using Inspect element in the browser found a line which serializes and base64 encoded. In that line it is mentioned and it encodes the browser cookie session

Taking the browser cookie session and decoding with base64 decoder.
I got this serialized code

``` O:4:\"User\":2:{s:4:\"name\";s:5:\"guest\";s:4:\"role\";s:5:\"Guest\";} ```

By changing the name to hqadmin and role to Administrator again base 64 encode and paste it in a cookie using any “cookie editor” You will get the flag for this Question.

### 3) Salty Spill


![1673364211527-nize](https://user-images.githubusercontent.com/53529867/211591755-f3ee4c2f-6346-47d2-a8db-6d52fcd9bccc.png)



### 4) Pail Pigment

![1673364423262-ultra-nize](https://user-images.githubusercontent.com/53529867/211592307-de38d255-4005-42dd-9e58-1d7ffb8dab63.png)

### 5) Intangible Momento

![1673364565085-super-nize](https://user-images.githubusercontent.com/53529867/211592984-7f7f5658-0001-42f5-a533-86689276993b.png)

### 6) Querier 

![1673364900226-nize](https://user-images.githubusercontent.com/53529867/211594400-757a6e15-7faf-4b90-b29b-87c11e237886.png)

### 7) Lame Rev

![1673365127190-super-nize](https://user-images.githubusercontent.com/53529867/211595246-cb4df321-7e4c-4b76-8e66-dd2c64d1972f.png)

# Do Check the CTF writeup File
