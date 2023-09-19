# Rammstein

## A Simple Git Tutorial & Markdown Guied

Generating a new SSH key
```hs
ssh-keygen -t ed25519 -C "your_email@example.com"
```
Adding your SSH key to the ssh-agent
```hs
eval "$(ssh-agent -s)"
```

```hs
ssh-add ~/.ssh/id_ed25519
```
Installing Git

```hs
sudo pacman -S git
```
Configuring Git

```hs
git config --global user.name "Your Name"
```
```hs
git config --global user.email "your.email@example.com"
```
Creating a Repository

```hs
git init
```
Cloning a Repository
```hs
git clone <repository_url>
```
Git Remote
```hs
git remote add <new_git-Repo-url>
```
```hs
git remote -v
```
```hs
git push origin main
```

Checking Status
```hs
git status
```

Adding Changes
```hs
git add .
```

Committing Changes
```hs
git commit -m "Your commit message"
```

Branches
```hs
git branch <branch_name>
```
```hs
git checkout <branch_name>
```
```hs
git checkout -b <new_branch_name>
```

Merging Branches

```hs
git merge <branch_name>
```

Pushing and Pulling
```hs
git push origin main
```
```hs
git pull origin main
````
Git Log
```hs
git log
```





## Headings﻿

# Heading 1
## Heading 2
### Heading 3
#### Heading 4
##### Heading 5
###### Heading 6

Heading 1 - Alternative Syntax
========

Heading 2 - Alternative Syntax
--------

## Paragraphs and Line Breaks﻿

Even though this text is written on two separate lines,
it is parsed as a single paragraph.

This paragraph is separated from the previous paragraph
by a blank line.

## Thematic Breaks

The underscores on the next line create a thematic break below this paragraph.
___
The minus signs below must be separated from this paragraph by a blank line.
If not, they are parsed as a level 2 heading.

----
Three or more asterisks also create a thematic break.
****

## Block Quotes

> Use quote blocks to emulate reply text.
> This line is part of the same quote.

This line is not formatted and does not belong to the quote block.

> This block spans multiple paragraphs.
>
> The second paragraph is grouped with the previous paragraph in the same quote block.
> Character formatting is _also_ supported inside the **quote block**.

> Quote blocks can also be nested.
>> When you start a new line with additional > characters,
>>> it simulates a threaded conversation.

## Indented Code Blocks

Start an indented code block following a paragraph with a blank line and at least four spaces of indentation:

    This is a code block.

    Blank lines between indented lines do not end the code block.

    Here is some HTML:
        <div class="footer">
            , ©,  2009—2017 JetBrains · All rights reserved
        </div>
This line of text is not indented. It ends the code block and starts a new paragraph.

## Fenced Code Blocks
Set multiple lines of code in fenced code blocks.

```
action: function(ctx) {
    workflow.check(!ctx.issue.isChanged('votes'), workflow.i18n('Voting for a resolved issue is not allowed.'));
},
```

The following code block uses syntax highlighting for Haskell:
```hs
-- Point-free style
fib :: Integer -> Integer
fib = (fibs !!)
where fibs = 0 : scanl (+) 1 fibs

-- Explicit
fib :: Integer -> Integer
fib n = fibs !! n
where fibs = 0 : scanl (+) 1 fibs
```

## Lists﻿

Things I need to do today:
1. Fix usability problem
2. Clean up the page
   * Make the headings bigger
2. Push my changes
3. Create code review
   * Describe my changes
   * Assign reviewers
     * Ask for feedback
    
## Tables

Kitchen Cleanup Rotation

| Month    | Assignee | Backup |
| -------- | -------- | ------ |
| January  | Dave     | Steve  |
| February | Gregg    | Karen  |
| March    | Diane    | Jorge  |

Here's the same text with character formatting.
+ The text in the first column is flush right.
+ The text in the second column is centered.
+ The Markdown is stripped down to the minimum syntax that is required to render the table.

Month | Assignee | Backup
---:|:---:| ---
**January** | Dave | _Steve_
**February** | Gregg | _Karen_
**March** | Diane | _Jorge_

## Links﻿

[inline link](https://www.github.com/mrsandaru)
[inline link with tooltip](https://www.github.com/mrsandaru "Git_Dot: My Git and Dot File Repo")
[reference link][1]

[1]: https://www.github.com/mrsandaru

## Autolinks

Both of these URLs are parsed as links:

<https://www.github.com/mrsandaru>
https://www.github.com/mrsandaru

Email addresses are also converted into "mailto" links when set in angle brackets:

<mrsanadru@github.com>

## Images 

Here's an image link to the Markdown logo on Wikipedia:

Inline:
![Markdown logo](https://upload.wikimedia.org/wikipedia/commons/3/35/Tux.svg "Linux")

Reference style:
![Markdown logo][logo]

[logo]: https://upload.wikimedia.org/wikipedia/commons/3/35/Tux.svg "Linux"

Markdown also supports images as links.
Just wrap the entire image reference in brackets then add the target URL in parenthesis after the image reference.
People use this syntax to insert a thumbnail image that links to a video on a video sharing platform.

But this is not a vedio:

[![YouTrack — Maintain Order In A World of Chaos](https://upload.wikimedia.org/wikipedia/commons/3/35/Tux.svg)](https://endeavouros.com/)

## Backslash Escapes﻿


Here are a few examples of backslash escapes:

\*not emphasis*
\`not an inline code span`
1\. not an ordered list
\* not an unordered list
\# not a heading

\This is not a backslash escape - the escaped character is not a markup character.
