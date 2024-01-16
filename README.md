# Github Maintain two remote url

- Vercel এ ফ্রি হোস্ট করার জন্য পার্সনাল একাউন্টের প্রাইভেট রিপোজিটরি 


## নিচের কমান্ড গুলো ফলো করুন :

```
git init

```

```
git add .

```

```
git commit -m "First commit"

```

```
git branch -M main

```

```
git remote add vercel YOUR_PERSONAL_ACCOUNT_REPOSITORY_HTTPS_URL

```

```
git remote add code LWS_CLASSROOM_REPOSITORY_HTTPS_URL

```

```
git push vercel main

```

```
git push code main

```

- মনে রাখবেন পুশ করার সময় খেয়াল রাখবেন আপনি কোন ব্রাঞ্চে আছেন আর কোন ব্রাঞ্চে পুশ করতেছে। **Git bash** Terminal এ দেখতে পারবেন আপনি কোন ব্রাঞ্চে আছেন বর্তমানে।
এরকম হলে ব্রাঞ্চ পরিবর্তন করে আবার পুশ করেন।

```
git branch -M main

```

এর পরেও না হলে:

- `.git` হিডেন ফোল্ডার ডিলিট দিয়ে আবার চেষ্টা করুন।

বিঃ দ্রঃ মনে রাখতে হবে কোনো কিছু পুশ করলে আপনাকে ২টা রিপোজিটরিতে পুশ করতে হবে। Deploy করার পরে গিটে আবার পুশ করলে vercel এ অটো আপডেট হয়ে যাবে।

## Git & GitHub Documentation:
```
   There is a dreamy boy whose name is bappa saha.

```
#  ⚙ 𝐆𝐢𝐭𝐡𝐮𝐛 branch delete  𝐫𝐮𝐥𝐞 :

   local:git branch -d  Transport-Component-POST--3.2
   
   remote:git push origin :Transport-C0mponent-3.2

# ⚙ 𝐆𝐢𝐭𝐡𝐮𝐛 𝐫𝐞𝐩𝐨𝐬𝐢𝐭𝐨𝐫𝐲 𝐜𝐥𝐨𝐧𝐞 𝐫𝐮𝐥𝐞

### Command these five steps to clone a git repository

    1.  git clone --bare proHero-htpps/link
    2.  cd (and go to that clone .git folder)
    3.  git push --mirror my-htpps/link
    4.  git remote -v
    5.  git remote set-url origin my-htpps/link

</a>

# 𝐀𝐥𝐥 𝐫𝐢𝐠𝐡𝐭 𝐫𝐞𝐬𝐞𝐫𝐯𝐞𝐝 𝐛𝐲 𝐛𝐚𝐩𝐩𝐚 𝐬𝐚𝐡𝐚 | 𝐁𝐬𝐜 𝐢𝐧 𝐂𝐒𝐄 |𝐑𝐌𝐒𝐓𝐔




### [Lesson 2. Introduction to git and GitHub]()

1. git?
   - git is a version control software
   - It keep track of code changes
   - It helps to collaborate in a project
   - It is installed and maintained locally
   - It provides Command Line Interface (CLI)
   - Released in April 7, 2005
   - Developed by Linus Torvalds & Junio C Hamano
2. github?
   - GitHub is a hosting service where we can keep our git repositiory/folders
   - It is maintained on cloud/web
   - It provides Graphical User Interface (GUI)
   - Founded in 2008

<img src="./images/git and github.png" width="90%">
     
<br/>

### [Lesson 3. How to set git environment and configuration](https://youtu.be/vj5-nkhTRbo)

- Download and install git on your pc: https://git-scm.com/
- check git version: open terminal or cmd then use the command `git --version` to find out whether git is installed or not. if git is installed it will return a version number of git.

<br/>

git configuration

1.  check all configuartion options: `git config`
2.  set global user name and user email for all repository/git folders (if you want to set different username and email for different git repository then remove --global)
    - set global user name: `git config --global user.name "anisul-islam"`
    - set global user email: `git config --global user.email "anisul2010s@yahoo.co.uk"`
3.  list all git configuration:
    - list all the configuration: `git config --list`
    - list user name: `git config user.name`
    - list user email: `git config user.email`
4.  change global username & email
    - change global user name: `git config --global user.name "PUT_NEW_USER_NAME_HERE"`
    - change global user email: `git config --global user.email "PUT_NEW_USER_EMAIL_HERE"`

<br/>

### [Lesson 4. creating git repo and adding new files](https://youtu.be/oa6viOCTEeM)

1.  creating a git folder

- ls -a : list all files inside of a directory

  ```
  mkdir DIRECTORY_NAME_HERE
  cd DIRECTORY_NAME_HERE
  git init

  Example:
  mkdir notes
  cd notes
  git init
  ls -a
  ```

2.  adding new files in git folder

- git status : displays the state of the working directory and staging area

  ```
  ls -a
  touch fileName.extension
  open fileName.extension
  git status

  Example:
  touch day1.txt
  open day1.txt
  write something inside the file
  ```

- Git is aware of the file but not added to our git repo
- Files in git repo can have 2 states – tracked (git knows and added to git repo), untracked (file in the working directory, but not added to the local repository)
- To make the file trackable stagging or adding is required

<br/>

### [Lesson 5. how to add files in staging area & remove files](https://youtu.be/IDhgZX4esQQ)

1.  adding files to stagging area:

- `git add fileName` add a file in staging area / index
- `git add .` add all files of directory to stagging area not subdirectory
- `git add -A` add all files of directory and subdirectory to stagging area
- `git rm --cached fileName` unstage a file from staging area
- `git diff` - checking the differences of a staged file
- `git restore fileName` - restore the file

<br/>

### [Lesson 6. practice-1](https://youtu.be/jSj-GF-utls)

<br/>

### [Lesson 7. commit & uncommit](https://youtu.be/gmBKbxKGcn8)

- `git commit -m "message"` move the file to local repository from stagging area
- `git log` check the commit history
- `git reset --soft HEAD^` uncommit the commit in HEAD and move to staging area
- `git reset HEAD^` uncommit the commit in HEAD and move to unstaging / working area
- `git reset --hard HEAD^` uncommit the commit in HEAD and delete the commit completely with all the changes

<img src="./images/git-level.png" width="90%">

<br/>

### [Lesson 8. git HEAD and undo theory](https://youtu.be/xUNsecljvog)

- `git log --oneline`
- `git show`
- `git show HEAD^`
- `git show commit-id`
- `git checkout commit-id`
- `git checkout master`

<br/>

### [Lesson 9. git HEAD and undo practical](https://youtu.be/rEoeC-HBqws)

<br/>

### [Lesson 10. git revert]()

<br/>

### [Lesson 11. git ignore](https://youtu.be/CKla6oWTezM)

- create a .gitignore file and add the things you do not want to add in the stagging area
- Inside .gitignore we can keep secret files, hidden files, temporary files, log files
- `secret.txt` secret.txt will be ignored
- `*.txt` ignore all files with .txt extension
- `!main.txt` ignore all files with .txt extension without .main.txt
- `test?.txt` ignore all files like test1.txt test2.txt
- `temp/` all the files in temp folders will be ignored

<br/>

### [Lesson 12. how to create github repository and commits](https://youtu.be/HRVNOjl9e5U)

- sign in to your github account
- create a git repo

<br/>

### [Lesson 13. README.md](https://youtu.be/bl0-DTgh-mw)
[README video is here](https://youtu.be/bl0-DTgh-mw)
- Everything you need to know about README.md is discussed in the video.
- 6 heading levels: number of hashes define heading levels. check the following examples:
  - `# heading 1 level text is here`
  - `## heading 2 level text is here`
- bold syntax: `**text goes here**`
- italic syntax: `_text goes here_`
- bold and italic syntax: `**_text goes here_**`
- strikethrouh syntax: `~~this is~~`
- single line code syntax: `` place code inside backticks
- multiple line code syntax: ``` place code inside three open and closing backticks 
            
- multiple line code syntax language specific: ```html for specific lanaguage use language name when starting; not closing
           
- Ordered List syntax 
      
      ```
           1. HTML
            2. CSS

               1. Fundamental
               2. CSS Architecture - BEM
               3. CSS Preprocessor - SASS

            3. JS
      ```
- Unordered List syntax -> 
     ```
      - html
      - css
        - Fundamental
        - CSS Architecture - BEM
        - CSS Preprocessor - SASS
      - js
     ```
- Task List 
   ```
      - [x] Task1
      - [x] Task2
      - [x] Task3
   ```
   
- adding link
   ```
      <!-- automatic link -->

      http://www.studywithanis.com

      <!-- markdown link syntax -->
      [title](link)
      [studywithanis](http://www.studywithanis.com)  
      [studywithanis][websitelink]

      <!-- all link is here  -->

      [websitelink]: http://www.studywithanis.com

- adding image syntax -> `![alt text](imageURL)`
      `![1800 milestone](https://i.postimg.cc/qvZpmxKF/1-800-Uploads-Milestone.png)`

- adding emoji   
      [emoji src](https://getemoji.com/)
      ### Smileys
      😀 😃 😄 😁 😆 😅 😂 🤣 🥲 ☺️ 😊 😇 🙂 🙃 😉 😌 😍 🥰 😘 😗 😙 😚 😋 😛 😝 😜 🤪 🤨 🧐 🤓 😎 🥸 🤩 🥳 😏 😒 😞 😔          😟 😕 🙁 ☹️ 😣 😖 😫 😩 🥺 😢 😭 😤 😠 😡 🤬 🤯 😳 🥵 🥶 😱 😨 😰 😥 😓 🤗 🤔 🤭 🤫 🤥 😶 😐 😑 😬 🙄 😯 😦 😧 😮       😲 🥱 😴 🤤 😪 😵 🤐 🥴 🤢 🤮 🤧 😷 🤒 🤕 🤑 🤠 😈 👿 👹 👺 🤡 💩 👻 💀 ☠️ 👽 👾 🤖 🎃 😺 😸 😹 😻 😼 😽 🙀 😿 😾

      ### Gestures and Body Parts
      👋 🤚 🖐 ✋ 🖖 👌 🤌 🤏 ✌️ 🤞 🤟 🤘 🤙 👈 👉 👆 🖕 👇 ☝️ 👍 👎 ✊ 👊 🤛 🤜 👏 🙌 👐 🤲 🤝 🙏 ✍️ 💅 🤳 💪 🦾 🦵 🦿 🦶      👣 👂 🦻 👃 🫀 🫁 🧠 🦷 🦴 👀 👁 👅 👄 💋 🩸
      
- adding table 
   ```
      table syntax
      | heading1 | heading2 |
      | ----- | ----- |
      | data1 | data2 |
      | data3 | data4 |
      | data5 | data6 |
   ```

<br>

### [Lesson 14. Connecting local repo to remote repo](https://youtu.be/sLX2YWYpkAc)

- check remote connection: `git remote` or `git remote -v`
- `git remote add name <REMOTE_URL>` example: git remote add origin http://...
- to clone a remote repository: `git clone <REMOTE_URL>`

<br>

### [Lesson 15. push and pull](https://youtu.be/UXEoCfYwI1Q)

- push a branch `git push -u origin branch_name`
- push all branches `git push --all`
- pull from a repo: `git pull` which is equivalent to git fetch + git merge

<br>

### [Lesson 16. branching and merging](https://youtu.be/3k8Bq_usPsk)

- Branch is a new and separate branch of master/main repository
- create a branch `git branch branch_name`
- List branches `git branch`
- List all remote branches `git branch -r`
- List all local & remote branches `git branch -a`
- move to a branch `git checkout branch_name`
- create and move to a branch `git checkout -b branch_name`
- delete a branch: `git branch -d branch_name`
- merge branches:
  ```
    git checkout branchName
    git merge branchName
  ```
- `git log --oneline --all --graph`

<br>

### [Lesson 17. branching and merging locally](https://youtu.be/AhBxGYzdWI0)

<br>

### [Lesson 18. git and GitHub practice - 2](https://youtu.be/IHVzseHh3Bo)

<br>

### [Lesson 19. GitHub Issues](https://youtu.be/E5HFlpx7QP4)

<br>

### [Lesson 20. 2-way and 3-way merges]()

- Reeference:
  - https://www.tutorialspoint.com/what-is-a-fast-forward-merge-in-git
  - https://www.tutorialspoint.com/what-is-3-way-merge-or-merge-commit-in-git
  - https://medium.com/@koteswar.meesala/git-fast-forward-merge-vs-three-way-merge-8591434dd350

<br>

### [Lesson 21. Merge Conflicts]()

- https://www.tutorialspoint.com/what-is-merge-conflict-in-git-how-to-handle-merge-conflicts

<br>

# Learn Markdown

[![Youtube Channel](https://img.shields.io/badge/Darun%20IT-Subscribe-red)](https://www.youtube.com/darunit "My youtube Channel")

[//]: # (Table of Content)

<a name="top"></a>

## Table of Markdown content

>Click on any topic to go there

1. [What is Markdown](#markdown)

1. [Heading](#heading)

1. [Comment](#comment)

1. [Text Formatting](#textformat)

1. [Escaping](#escap)

1. [Blockquote](#quote)

1. [Strikethrough](#strike)

1. [Horizontal Line](#horiline)

1. [List](#list)

1. [Link](#link)

1. [Emoji](#emoji)

1. [Image](#image)

1. [Table](#table)

1. [Code Block](#codeb)

1. [Fancy Code Block](#fcodeb)

1. [Collapsible Content](#collap)

1. [Check Box](#check)

1. [Keyboard Button](#btn)

1. [Badge](#badge)

1. [Mention](#mention)

1. [Learning Links](#learning)

---
***


[//]: # (What is Markdown)

<a name="markdown"></a>

# What is Markdown?

Markdown is the formatting elements to plaintext text documents.Markdown documents are readable without tags. Behind the seen it has been converted to html. It use to style text,list, table etc.You can consider markdown as regular text.

---
___

<!-- What is Markdown End -->


[//]: # (Heading Syntax)

<a name="heading"></a>



# Heading Syntax of Markdown

```
###### Heading-6
##### Heading-5
#### Heading-4
### Heading-3
## Heading-2
# Heading-1
```
**Example of markdown heading**

###### Heading-6
##### Heading-5
#### Heading-4
### Heading-3
## Heading-2
# Heading-1

```
You can use this heading-1 syntax
=================================
```
**Example**

You can use this heading-1 syntax
=================================

```
You can use this heading-2 syntax
---------------------------------
```
**Example**

You can use this heading-2 syntax
---------------------------------

[Go to top:arrow_up: ](#top)

***
***
<!-- Heading Syntax End -->

[//]: # (Comment syntax)

<a name="comment"></a>

# Comment Syntax of Markdown

```
[//]: # (This is recommended Comment Syntax)

[comment]: <> (You can use this comment syntax)

[//]: <> (This is another comment syntax)
```

[Go to top:arrow_up: ](#top)

---
---
<!-- Comment Syntax End -->

[//]: # (Text Formatting Syntax)

<a name="textformat"></a>

# Text Formatting Syntax of Markdown
## Bold text
```
**Bold text with 2 stars in both side**
__Bold text with 2 underscore in both side__
```
### Example

**This is Bold text example with 2 stars**

__This is Bold text example with 2 underscore__

I love **B**angladesh

We are learning **markdown** language

> *Double underscore not work to bold

I love __B__angladesh

## Italic Text
```
*Italic text with 1 star in both side*
_Italic text with 1 underscore in both side_
```
### Example

*This is Bold text example with 2 stars*

_This is Bold text example with 2 underscore_

## Bold & Italic at a time
```
***Bold italic text Syntax***

___Bold italic text Syntax___

*__Bold italic text Syntax__*

_**Bold italic text Syntax**_
```
### Example

***Bold italic text***

___Bold italic text___

*__Bold italic text__*

_**Bold italic text**_

## Paragraph
**Line Breack**

The world's eighth largest country in population Bangladesh , although the size of small islands <br></br> city-states after the 9 th 6 of the world's most densely populated country, Bangladesh . With an estimated population (2016) of this small country of less than 56,000 square miles,

the population is more than 160 million, or 279 people per square mile (1115 people per square kilometer).

**Way to center text**

<p align="center">
The world's eighth largest country in population Bangladesh , although the siaze of small islands and city-states after the 9 th 6 of the world's most densely populated country, Bangladesh . With an estimated population (2016) of this small country of less than 56,000 square miles, the population is more than 160 million, or 279 people per square mile (1115 people per square kilometer).
</p>


[Go to top:arrow_up: ](#top)

___
___
<!-- Text Formatting Syntax End -->

[//]: # (Escaping Syntax)

<a name="escap"></a>

# Escaping Syntax of Markdown

```\# Backslash escape to work```

**Example**

\# Backslash escape to work

\- Backslash escape to work

\\* Backslash escape to work

[Go to top:arrow_up: ](#top)

---
---
<!-- Escaping Syntax End -->


[//]: # (Blockquote Syntax)

<a name="quote"></a>

# Blockquote Syntax of Markdown

>This is blockquote
>>Inside the Parent
>>> Inside the 2nd parent
>
>This is blockquote
>>Inside the parent
>>>Inside the 2nd parent

>One line gap to create new blockquote

[Go to top:arrow_up: ](#top)

***
___
<!--Blockquote Syntax End  -->

[//]: # (Strikethrough Syntax)

<a name="strike"></a>

# Strikethrough Syntax of Markdown

```
~~Line cutted~~
```
**Example**

~~Line cutted~~

[Go to top:arrow_up: ](#top)
___
***
<!-- Strikethrough Syntax End -->

[//]: # (Horizontal Line Syntax)

<a name="horiline"></a>

# Horizontal Line Syntax of Markdown

```
---
***
___
```
**Example**

---
***
___

[Go to top:arrow_up: ](#top)

---
***

<!-- Horizontal Line Syntax End-->

[//]: # (List Syntax)

<a name="list"></a>

# List Syntax of Markdown

**Order list**

```
1. Jubaer
1. Mohammad
1. Mitu
1. Bizly
```
**Example**

1. Jubaer
1. Mohammad
1. Mitu
1. Bizly

**Unodder list**

```
- Akter Hossain
* Arif Hossain
+ Korim Hossain
```

**Example**

- Akter Hossain
* Arif Hossain
+ Korim Hossain

[Go to top:arrow_up: ](#top)
___
***
<!-- List Syntax End -->

[//]: # (Link Syntax)

<a name="link"></a>

# Link Syntax of Markdown

```
[Link Text](https://www.darunit.com "Visit Boos")

To know more about us visit [Darun IT]

[Darun IT]: https://www.darunit.com "Visit"
```
**Example**

[Link Text](https://www.darunit.com "Visit Boos")

To know more about us visit [Darun IT]

[Darun IT]: https://www.darunit.com "Visit"


[Go to top:arrow_up: ](#top)
___
***
<!-- Link Syntax End -->

[//]: # (Emoji Syntax)

<a name="emoji"></a>

# Emoji Syntax of Markdown

```
:heart: you can copy only emoji 💬
```
**Example**

:heart: you can copy only emoji 💬

[Go to top:arrow_up: ](#top)

***
---
<!-- Emoji Syntax End -->


[//]: # (Image Syntax)

<a name="image"></a>

# Image Syntax of Markdown

```
![Darun IT Logo](logo.png "Logo")
```

**Example**

![Darun IT Logo](logo.png "Logo")

**Linkable Image**
```
[![Darun IT Logo](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTZVBxXXB2ET_ZNUuNzOE7mvx1fnYOSiUmPzA&usqp=CAU "Download Icon")](https://www.fb.com "Click to download")
```

**Way to center image**

<p align="center">
<img src="logo.png" width="60%" align="">
</p>

[Go to top:arrow_up: ](#top)

---
***
<!-- Image Syntax End -->

[//]: # (Table Syntax)

<a name="table"></a>

# Table Syntax of Markdown

```
No | Icon | Shortcode
---|------|----------
01 | ❤️  | `:heart:`
02 | 👁️‍🗨️  | `:eye_speech_bubble:`
03 | 👍  | `:+1:`
```
**Example**

No | Icon | Shortcode
---|------|----------
01 | ❤️  | `:heart:`
02 | 👁️‍🗨️  | `:eye_speech_bubble:`
03 | 👍  | `:+1:`

[Go to top:arrow_up: ](#top)
___
***
<!-- Table Syntax End -->

[//]: # (Code Block Syntax)

<a name="codeb"></a>

# Code Block Syntax of Markdown

**Inline Code Block**

```
This is a variable `let name = "Jubaer"`
```
##### Example

This is a variable `let name = "Jubaer"`

**Multi Line Code Block**

```
```Use 3 backtick for multi line code block
<body>
        <h1>Html code</h1>
</body>```
```

**Example**

```
function fancyAlert(arg) {
  if(arg) {
    $.facebox({div:'#foo'})
  }
}
```

[Go to top:arrow_up: ](#top)

___
***
<!-- Code Block Syntax End -->

[//]: # (Fancy Code Block)

<a name="fcodeb"></a>

# Fancy Code Block of Markdown

```
```javascript
function fancyAlert(arg) {
  if(arg) {
    $.facebox({div:'#foo'})
  }
}```
```
**Example**

```javascript
function fancyAlert(arg) {
  if(arg) {
    $.facebox({div:'#foo'})
  }
}
```
[Go to top:arrow_up: ](#top)

___
***
<!-- Fancy Code Block End -->

[//]: # (Collapsible Content)

<a name="collap"></a>

# Collapsible Content of Markdown

```
<details>
    <summary>About Jubaer Ahmad</summary>

 # His education

 Jubaer Ahmad is a full stack web developer.
 He love to teach people, he is expart in javascript, php and markdown 
</details>
```

**Example**

<details>
    <summary>About Jubaer Ahmad</summary>

 # His education

 Jubaer Ahmad is a full stack web developer.
 He love to teach people, he is expart in javascript, php and markdown 
</details>

[Go to top:arrow_up: ](#top)
___
---
<!-- Collapsible Content End -->

[//]: # (Check Box Syntax)

<a name="check"></a>

# Check Box Syntax of Markdown

```
- [ ] Check Box
- [x] Check Box
```

**Example**

- [ ] Check Box
- [x] Check Box

[Go to top:arrow_up: ](#top)

***
---
<!-- Check Box End -->

[//]: # (Keyboard Button)

<a name="btn"></a>

# Keyboard Button of Markdown

```
To Select All: <kbd>CTRL</kbd> + <kbd>A</kbd>
```
**Example**

To Select All: <kbd>CTRL</kbd> + <kbd>A</kbd>

[Go to top:arrow_up: ](#top)

---
***
<!-- Keyboard Button End -->


[//]: # (Badge Syntax)

<a name="badge"></a>

# Badge Syntax of Markdown

```
[![Youtube Channel](https://img.shields.io/badge/Darun%20IT-Subscribe-red)](https://www.youtube.com/darunit "My youtube Channel")
```
**Example**

[![Youtube Channel](https://img.shields.io/badge/Darun%20IT-Subscribe-red)](https://www.youtube.com/darunit "My youtube Channel")


[Go to top:arrow_up: ](#top)
___
---
<!-- Badge Syntax End -->

[//]: # (Mention Syntax)

<a name="mention"></a>

# Mention Syntax of Markdown

> Use @ to mention a user on gitgub

**Example**

@JubaerAhmad

[Go to top:arrow_up: ](#top)

---
---
<!-- Mention Syntax End -->

[//]: # (Learning Links)

<a name="learning"></a>

# Learning Links of Markdown

- [Markdown Video in bangla](https://youtu.be/7TWhI3kemVM)

- [Bangla Cheat Sheet](https://devsonket.com/markdown/)

+ [Emoji Link](https://github.com/JubaerAhmad/gitgub-emoji#table-of-contents)

* [Mastering Markdown](https://guides.github.com/features/mastering-markdown/#GitHub-flavored-markdown)

- [Badge Website Link](https://shields.io/)

- [Markdown Online Editor](https://stackedit.io/)

- [Diagram Website Link](https://mermaid-js.github.io/mermaid/#/)

- [README.MD Stats Link](https://github.com/anuraghazra/github-readme-stats)
- [Visualizing-Git](https://git-school.github.io/visualizing-git/)

[Go to top:arrow_up: ](#top)

---
---
<!-- Learning Links End -->

This content is written by [Jubaer Ahmad](https://www.facebook.com/JubaerAhmad.info "This is my fb page link")

---
***


###   copyright by anis vai.
