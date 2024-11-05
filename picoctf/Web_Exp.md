# SOAP

**Flag:** `flag`

How you approached the challenge:

- step 1

```
code
```

- step 2

```
terminal output
```

- etc.

![screenshot](./.png)

What you learned through solving this challenge:

1. first concept
2. second concept
3. etc.

Other incorrect methods you tried:

- a
- b
- c

References

- reference 1
- reference 2
- etc.


# Forbidden Paths

**Flag:** `picoCTF{7h3_p47h_70_5ucc355_6db46514}`

How you approached the challenge:

- Step 1:
Looking at the challenge prompt and specifically at `/usr/share/nginx/html/`, I realised I had to use relative paths to get to `flag.txt` 

- Step 2:
Keep adding `../` with the file to keep moving backwards into the parent directory and see if I get a response

- Step 3:
Retrieve the flag using the final prompt as `../../../flag.txt`
![screenshot](./screenshot.png)

What you learned through solving this challenge:

1. Relative file paths and their usage

Other incorrect methods you tried:

- a. Directly trying to run `/flag.txt` or just `flag.txt` 
- b. Going through source code to find a hidden file
- 

# cookies

**Flag:** `picoCTF{3v3ry1_l0v3s_c00k135_bb3b3535}`

How I approached the challenge:
- Step 1: 
On opening the website and considering the name of the challenge _cookies_, it pointed to looking at the cookies of the website

- Step 2: 
Open the "Inspect element" tab (also known as the developer tools) using ` Ctrl + Shift + I ` and head to the ` Application ` tab

- Step 3: 
Looking at the cookie data, I noticed a pre defined cookie call `name` with a value of `-1`

- Step 4: 
Looking at the already given name for the cookie ptompt as "snickerdoodle", I put it into to input field and realised that the `name ` cookie had its value updated to `0`. </br>  </br> **BINGO**

- Step 5: 
Increment the value of the `name` cookie by 1 to see how the output changes
2: Oatmeal raisin
3: gingersnap
4: shortbread
5: peanut butter cookies
6: whoopie pie cookies
7: sugar 
8: molasses cookies
and so on

This went on upto value of 18 where it gave the flag

![screenshot](./cookies_ss.png)

What you learned through solving this challenge:

1. Going through cookies and editing thier values

Other incorrect methods you tried:

- a. Looking through the source code for any clue of the value, but ended up brute forcing it

