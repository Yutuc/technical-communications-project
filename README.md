# How to host & format a resume using Markdown, VSCode, GitHub Pages, and Jekyll

## Purpose

The purpose of this document is to convince readers, especially software developers, into creating simple, elegant, and customizable resumés. Specifically, using current technical documentation tools such Markdown, VSCode, GitHub Pages, and Jekyll as  described in Andrew Etter's book, _Modern Technical Writing: An Introduction to Software Documentation_. Additionally, this tutorial will introduce and demonstrate key principles mentioned in Etter's book. These principles are particularily useful for computer science students as they describe comprehensive guidelines in creating effective documentation. This is a skill software developers in the workforce inevitably are required to learn and master. This stems from the fact that good documentation encourages and simplifies collaboration between software developers in teams; which is a common environment for developers.

## Getting Started

Now, I understand some of you may not have any experience in Markdown, VSCode, GitHub Pages, or Jekyll. This is totally okay! This tutorial will comprehensively go through each step while explaining how it relates to Etter's protocol. First, let us start with a couple of prerequisites. 

### Prerequisites

#### Markdown
First, you need to learn Markdown. Specifically, GitHub Flavored Markdown. Markdown is the most widely used lightweight markup language. Additionally, out of the lightweight markup languages, Markdown has the "cleanest syntax" (Etter, 2016, p. 21). However, it has drawbacks such as limited features, which makes customizing the aesthetics of your document difficult. Also, there is no universally agreed upon standard, which means users may have to convert their document to other Markdown flavors to make it compatible with certain websites.

Since we are going to be hosting this project using GitHub Pages, I recommend getting familiar with GitHub Flavored Markdown. To learn Markdown, you can use either of the following links below: 
- [GitHub Flavored Markdown](https://www.example.com)
- [Vanilla Markdown](https://www.markdowntutorial.com/lesson/1/)

#### VSCode
Next you need to a Markdown editor. I recommend using VSCode with a Markdown viewer extension. 

1. Install VSCode through this [link](https://code.visualstudio.com/)
2. Then install the Markdown Preview Enhanced extension by Yiyi Wang

    ![Installing Markdown Preview Enhanced](https://upload.wikimedia.org/wikipedia/commons/5/56/Tiger.50.jpg)
3. You may now edit Markdown files and see how they will be rendered in real time

    ![Using Markdown Preview Enhanced Extension](https://upload.wikimedia.org/wikipedia/commons/5/56/Tiger.50.jpg)

#### Resumé
Once you know Markdown and have a Markdown editor to use, create a Markdown formatted resumé for yourself. 

#### Jekyll
If you are happy with using any of these GitHub Pages supported Jekyll [themes](https://pages.github.com/themes/) then you may skip this section. Otherwise, you will need to install Jekyll locally to be able to use custom Jekyll themes from other sources. Choose your operating system below and follow the installation steps.
- [Windows](https://jekyllrb.com/docs/installation/windows/)
- [macOS](https://jekyllrb.com/docs/installation/macos/)
- [Ubuntu](https://jekyllrb.com/docs/installation/ubuntu/)
- [Other Linux](https://jekyllrb.com/docs/installation/other-linux/)

## How to host a Markdown resumé on GitHub Pages

Great job so far! It is now time for the real fun stuff. Now, let us explore how each component in our software stack interact with each other and how each of them relates back to Etter's protocol.

### GitHub Version Control
__Explain why using GitHub, specifically version control, is useful and relate it to Andrew Etter's book.__

1. Create a GitHub account [here](https://github.com/signup?ref_cta=Sign+up&ref_loc=header+logged+out&ref_page=%2F&source=header-home) if you do not already have one
2. [Sign in](https://github.com/login?return_to=https%3A%2F%2Fgithub.com%2Fsignup%3Fref_cta%3DSign%2Bup) to your new GitHub account
    Your dashboard should look something like this (left navigation bar will be empty if your account is new):

    ![GitHub Dashboard](https://upload.wikimedia.org/wikipedia/commons/5/56/Tiger.50.jpg)
3. Create a new repository
    * Make sure to make your repository name __\<username\>.github.io__ in this format
    * For example, if my username was JohnDoe then my repository name would be __johndoe\.github\.io__
    * __Explain why this naming convention is useful__

    ![Creating a new respository](https://upload.wikimedia.org/wikipedia/commons/5/56/Tiger.50.jpg)
4. Download your repository into your local system

    ![Download your repository](https://upload.wikimedia.org/wikipedia/commons/5/56/Tiger.50.jpg)
5. Open your repository folder in VSCode

    ![Open repository in VSCode](https://upload.wikimedia.org/wikipedia/commons/5/56/Tiger.50.jpg)

6. Next, with your project's repository still open in VSCode, you are going to create __3__ new files:
    1. index\.md
        * This is the file where you will type your Markdown resumé in
    2. _config.yml
        * This file will control what Jekyll theme will be applied/rendered with your index\.md file
    3. README\.md
        * This file is for any documentation you may want to include

    ![Creating necessary files](https://upload.wikimedia.org/wikipedia/commons/5/56/Tiger.50.jpg)
7. Commit your changes to your local git

    ![Git Commit](https://upload.wikimedia.org/wikipedia/commons/5/56/Tiger.50.jpg)
8. Push your changes to GitHub

    ![Git Push](https://upload.wikimedia.org/wikipedia/commons/5/56/Tiger.50.jpg)

9. You should now be able to see your new files in your repository in your GitHub account

    ![View new files in GitHub](https://upload.wikimedia.org/wikipedia/commons/5/56/Tiger.50.jpg)

### Markdown
__Markdown file, why is it fundamental to etters book, links to markdown tutorials, how to write a markdown file, why is this important to static sites, quote from andrew etters book__.
1. Placeholder text

### Hosting on GitHub Pages
__choosing a jekyll theme, relate to etters book, relate static site generators like jekyll and why its mportant to andrew etters book__
1. Navigate to the __Settings__ tab in your repository
2. Then click the __Pages__ tab on the left navigation bar
3. Within the __Pages/GitHub Pages__ tab set the __Source__ to be __master/root__ or __main/root__, depending on how your GitHub is configured, and then press __Save__.
4. You may now view your static site at __https://\<username\>.github.io__
    * For example, if my username was JohnDoe then my static site will be published at  __https://johndoe\.github\.io/__

### Choosing your Jekyll theme
1. Navigate to the __Settings__ tab in your repository
2. Then click the __Pages__ tab on the left navigation bar
3. Within the __Pages/GitHub Pages__ tab 

### More Resources
  - [GitHub Flavored Markdown](https://www.example.com)
  - [Vanilla Markdown](https://www.markdowntutorial.com/lesson/1/)
  - [Modern Technical Writing: An Introduction to Software Documentation](https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS)
  - [VSCode](https://code.visualstudio.com/)
  - [Jekyll](https://jekyllrb.com/)
  - [Getting Started with GitHub Pages](https://guides.github.com/features/pages/)

## Authors

  - __Patrick Yutuc__ - *Provided all project files* - [Yutuc](https://github.com/Yutuc)


## Acknowledgments

  - __Asia Miyayi__ - *Editor*
  - __Humayra Rafi__ - *Editor*
  - __Kamarabbas Saiyed__ - *Editor*
  - __Joe Smith__ - *Editor*
  - __Billie Thompson__ - *Provided README Template* - [PurpleBooth](https://github.com/PurpleBooth)
  - __GitHub Pages__ - *Provided Slate Theme* - [Slate Theme](https://github.com/pages-themes/slate)

## FAQs (Frequently Asked Questions)

1. A question about the overall process, such as “Why is Markdown better than a word processor?”
2. A question about the practical details, such as “Why is my resume not showing up?”
