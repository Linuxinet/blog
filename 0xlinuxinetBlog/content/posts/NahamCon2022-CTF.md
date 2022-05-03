---
title: "NahamCon2022 CTF"
description: Blog Contains Solutions for NahamCon2022 CTF Challenges. 
date: 2022-05-01T16:36:29Z
---

# NahamCon2022 CTF

This Writeup Includes Solutions For Some of the Challenges.

## Challenges 

1. [Quirky](#quirky)
2. [Prisoner](#prisoner)
3. [Wizard](#wizard)
4. [Jurrasic Park](#jurrasic-park)
5. [Personnel](#personnel)
6. [When Am I](#when-am-i)
7. [One Mantissa Please](#one-mantissa-please)
8. [To Be And Not To Be](#to-be-and-not-to-be)
9. [Gossip](#gossip)
10. [Steam LocoMative](#steam-locomative)
11. [Keeber ( 1 - 8)](#keeber)


## Quirky

![Quirky Challenge](/quirky.png)

After Downloading the Challenge File `quirky` it contains the Following Hex Code

```
\x89\x50\x4e\x47\x0d\x0a\x1a\x0a\x00\x00\x00\x0d\x49\x48\x44\x52\x00\x00\x00\x6f\x00\x00\x00\x6f\x01\x03\x00\x00\x00\xd8\x0b\x0c\x23\x00\x00\x00\x06\x50\x4c\x54\x45\x00\x00\x00\xff\xff\xff\xa5\xd9\x9f\xdd\x00\x00\x00\x02\x74\x52\x4e\x53\xff\xff\xc8\xb5\xdf\xc7\x00\x00\x00\x09\x70\x48\x59\x73\x00\x00\x0b\x12\x00\x00\x0b\x12\x01\xd2\xdd\x7e\xfc\x00\x00\x01\x25\x49\x44\x41\x54\x38\x8d\xd5\xd4\x31\x8e\xc3\x20\x10\x05\xd0\xb1\x5c\xd0\x25\x17\x40\x9a\x6b\xd0\x71\x25\xfb\x02\xb6\xf7\x02\xce\x95\xe8\xb8\x06\x92\x2f\x40\x3a\x0a\x94\xd9\x8f\x23\x45\xbb\xc5\x66\x68\x52\x2c\xa2\xe0\x21\x21\xcf\x0c\x83\x49\x7e\x0d\xfa\x1f\xcc\x44\x8b\xaf\x6b\xb0\x44\xac\xf2\x2e\x75\x72\xe3\x66\xea\x2a\x1d\x0c\x76\xc1\xe7\x82\x9d\x4c\x17\x27\x97\xc8\xd4\x4e\xae\x91\xd6\x62\xbb\x28\x75\x8e\xf5\x1a\xed\x2b\xc8\x37\x44\xbe\x73\xb4\x98\xaf\xf4\xdf\xf0\x1c\xf6\x5a\x7e\x16\xf6\x4f\x66\xb2\x64\x78\xf3\xc7\xee\x3a\xe8\x0f\xac\x25\x10\x39\x56\x79\x2f\x74\x71\xe3\x57\x94\x87\x11\x9d\xf1\xd8\x5b\x6c\x34\x79\x9d\x0f\x8f\xb3\xb2\xfb\x73\x53\xa5\x3b\x36\x33\xa2\xf8\x73\x60\x95\x52\xea\x10\xd3\xc5\xf0\x7e\x46\xf5\x9e\x77\x19\x6f\x6d\x4a\x76\x3a\x25\xa0\x49\xda\x05\xdd\x22\xab\x44\xbe\x38\x28\x25\xcd\xa5\x83\x92\x86\x82\x90\x0e\x14\x53\x67\x44\x1f\xd6\x39\xa0\xfe\xac\xb3\x9d\x95\xdd\x10\x19\x51\x89\x91\x3d\x21\xa4\xec\x58\x25\x3a\x76\xf2\x69\x68\xaf\x4c\x54\xe2\x2d\x2c\x1e\x95\xe4\xec\x59\x27\xae\x52\xd0\xb4\x34\x3c\xf3\x55\x89\x85\xf0\xc3\x71\x17\x0b\xdf\x42\x22\x27\x3a\xf1\x7e\xd1\x2d\x68\xaa\xa2\xb3\xe5\xdb\x3a\x56\xb2\xd1\xf9\xb9\x5f\xee\xa7\xf8\x0d\x69\xf5\x37\x77\x6e\xf8\x09\x97\x00\x00\x00\x00\x49\x45\x4e\x44\xae\x42\x60\x82
```
Used Cyberchef To Decode the Hex

![quirky Cyberchef decode](/Quirky-cyber.png)

**Flag:** `flag{b7e2a32f5ae629dcfb1ac210d1f0c032}`

## Prisoner

![Prisoner Challenge](/prisoner.png)

After Connecting to the ssh it showing like this

![prisoner ssh](/prisoner-1.png)

Press `ctrl+c` now we break the console and landed in to python terminal
from that i got the shell and retrieved flag
`pty.spawn('/bin/sh')`

![prisoner flag](/prisoner-flag.png)

finally we got the flag

**Flag :** `flag{c31e05a24493a202fad0d1a827103642}`

## Wizard

![wizard challenge](/wizard.png)

this challenge contains some questions we need to answer

![wizard 1](/wizard1.png)

By Using Cyberchef We were able to complete first 2 questions

### 1 & 2

![wizard 2](/wizard2.png)

![wizard 3](/wizard3.png)

### 3
for 3rd question used <https://www.rapidtables.com/convert/number/octal-to-decimal.html> to solve the challenge

Octal -> Decimal 

Decimal -> Hex 

Hex -> Text

![wizard 4](/wizard4.png)

### 4

for the 4th question we need to convert the integer into hex and again convert the hex into text format

Decimal -> Hex -> Text

![wizard 6](/wizard6.png)

### 5

Decode Base64 string to plaintext

![wizard 7](/wizard7.png)

### 6

for the last question , it was somehow tricky, in this question we need to convert the little endian Hex string in Big endian Plain Text form, so first we need to convert the string from little endian to big endian hex string

_little endian Hex:_ `293a2065636e657265666669642065687420776f6e6b206f7420646f6f672073277449`

i used this online converter
<https://www.save-editor.com/tools/wse_hex.html>

_Big endian Hex:_ `4974277320676F6F6420746F206B6E6F772074686520646966666572656E6365203A29`

converted the Big endian Hex into plaitext

![wizard 8](/wizard8.png)

By solving the final question we got the flag

**Flag :** `flag{c2ed35aba037cd93381b298caa2720ee}`


## Jurrasic Park

![jurrasic park](/jurasicpark.png)

![jurasic](/jurasic1.png)

opened `robots.txt` found a directory 
![jurasic park robots.txt](/jurasicrobo.png)

found flag.txt in `/ingen/`  direcrory
![jirasic park index](/jurasicingen.png)

![flag.txt](/jurasicflag.png)


## Personnel

**app.py**


```python
#!/usr/bin/env python

from flask import Flask, Response, abort, request, render_template
import random
from string import *
import re

app = Flask(__name__)

flag = open("flag.txt").read()
users = open("users.txt").read()

users += flag


@app.route("/", methods=["GET", "POST"])
def index():
    if request.method == "GET":
        return render_template("lookup.html")
    if request.method == "POST":
        name = request.form["name"]
        setting = int(request.form["setting"])
        if name:
            if name[0].isupper():
                name = name[1:]

        results = re.findall(r"[A-Z][a-z]*?" + name + r"[a-z]*?\n", users, setting)
        results = [x.strip() for x in results if x or len(x) > 1]

        return render_template("lookup.html", passed_results=True, results=results)


if __name__ == "__main__":
    app.run()
```

as we can observe in the code it was taking our `name` parameter as a variable and giving output matches to the `name` variable

```python
results = re.findall(r"[A-Z][a-z]*?" + name + r"[a-z]*?\n", users, setting)
```
in this line the `name` variable was added in to the regex

so i used a regex pattern which matches to everything

**regex pattern:**
`[\s\S]*`

by using this regex as input the website shown all the content with flag 

**Flag:**
`flag{f0e659b45b507d8633065bbd2832c627}`

## When Am I
## One Mantissa Please
## To Be And Not To Be 
## Gossip
## Steam LocoMative
## Keeber
