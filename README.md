# How to host & format a resume using Markdown, VSCode, GitHub Pages, and Jekyll

## Purpose

The purpose of this document is to convince readers, especially software developers, into creating simple, elegant, and customizable resumés. Specifically, using current technical documentation tools such Markdown, VSCode, GitHub Pages, and Jekyll as  described in Andrew Etter's book, _Modern Technical Writing: An Introduction to Software Documentation_. Additionally, this tutorial will introduce and demonstrate key principles mentioned in Etter's book. These principles are particularily useful for computer science students as they describe comprehensive guidelines in creating effective documentation. This is a skill software developers in the workforce inevitably are required to learn and master. This stems from the fact that good documentation encourages and simplifies collaboration between software developers in teams; which is a common environment for developers.

## Getting Started

Now, I understand some of you may not have any experience in Markdown, VSCode, GitHub Pages, or Jekyll. This is totally okay! This tutorial will comprehensively go through each step while explaining how it relates to Etter's protocol. First, let us start with a couple of prerequisites. 

### Prerequisites

#### VSCode
First, you are going need to a Markdown editor. I recommend using VSCode with a Markdown viewer extension. 

1. Install VSCode through this [link](https://code.visualstudio.com/)
2. Then install the Markdown Preview Enhanced extension by Yiyi Wang

    ![Installing Markdown Preview Enhanced](https://i.imgur.com/CafrpvT.jpeg)
4. Click the Markdown Preview button on the top right corner

    ![Markdown Preview Button](https://i.imgur.com/r2wHM6u.jpg)
3. You may now edit Markdown files and see how they will be rendered in real time

    ![Using Markdown Preview Enhanced Extension](https://i.imgur.com/a1BVtkK.jpg)

#### Resumé
You need to learn Markdown and have a Markdown editor to use. Then create a Markdown formatted resumé for yourself. 

Since we are going to be hosting this project using GitHub Pages, I recommend getting familiar with GitHub Flavored Markdown. To learn Markdown, you can use either of the following links below: 
- [GitHub Flavored Markdown](https://www.example.com)
- [Vanilla Markdown](https://www.markdowntutorial.com/lesson/1/)

## How to host a Markdown resumé on GitHub Pages

Great job so far! It is now time for the real fun stuff. Now, let us explore how each component in our software stack interact with each other and how each of them relates back to Etter's protocol.

### GitHub Version Control

#### Why GitHub?

Version control is important to documentation because as products/software changes, so does the corresponding documentation. Version control also makes it easy to keep our documentation up to date and enables other developers to make suggestions to improve our documentation. In our case, we will store our documentation in the same repository its corresponding source code. As Etters (2016) explains, this approach has appeal to softawre developers as the "documentation and code branches stay in sync" and "developers are more likely to contribute if they don't have to clone a separate repository". We will be using GitHub due to the fact that it collaborates beautifully with GitHub Pages and Jekyll. 

#### Instructions

1. Create a GitHub account [here](https://github.com/signup?ref_cta=Sign+up&ref_loc=header+logged+out&ref_page=%2F&source=header-home) if you do not already have one
2. [Sign in](https://github.com/login?return_to=https%3A%2F%2Fgithub.com%2Fsignup%3Fref_cta%3DSign%2Bup) to your new GitHub account
    Your dashboard should look something like this (left navigation bar will be empty if your account is new):

    ![GitHub Dashboard](https://i.imgur.com/gDiaDpV.jpg)
3. Create a new repository
    ![Creating a new repository](https://i.imgur.com/iC4PkgP.jpg)
    ![Initial repository screen](https://i.imgur.com/TKA15WU.jpg)
    * Make sure to make your repository name __\<username\>.github.io__ in this format
    * For example, if my username was JohnDoe then my repository name would be __johndoe\.github\.io__
    * This naming format is important because GitHub will recognize you want to create a static website and make the URL for this repository __https://\<username\>.github.io__

    
4. Clone your repository into your local system

    ![Cloning repository](https://i.imgur.com/E7cqNN4.gif)
5. Open your recently cloned repository folder in VSCode

### Markdown

#### Why Markdown?
First, you need to learn Markdown. Specifically, GitHub Flavored Markdown. Markdown is the most widely used lightweight markup language. Lightweight markup languages like Markdown are an important piece to static sites as they provide the content without having to learn more cumbersome languages like HTML and CSS. Additionally, out of the lightweight markup languages, Markdown has the "cleanest syntax" (Etter, 2016, p. 21). Markdown is great for creating content for static websites because it is quick, simple, and secure (Etter, 2016, p. 26). However, it has drawbacks such as "limited features" (Etter, 2016, p. 21), which makes customizing the aesthetics of your document difficult. Also, there is no universally agreed upon standard, which means users may have to convert their document to other Markdown flavors to make it compatible with certain websites (Etter, 2016, p. 21).

To reiterate, you can use either of the following links below to learn Markdown: 
- [GitHub Flavored Markdown](https://www.example.com)
- [Vanilla Markdown](https://www.markdowntutorial.com/lesson/1/)

#### Instructions

1. Next, with your project's repository still open in VSCode, you are going to create __3__ new files:
    1. __index\.md__
        * This is the file where you will type your Markdown resumé in

        ![Resume typing demo](https://i.imgur.com/H5sfEvT.gif)
    2. ___config.yml__
        * This file will control what Jekyll theme will be applied/rendered with your index\.md file
    3. __README\.md__
        * This file is for any documentation you may want to include

2. Commit your changes to your local git

    ![Git Commit](https://i.imgur.com/8IFlG0p.gif)
3. Push your changes to GitHub

    ![Git Push](https://i.imgur.com/ZX0V28Y.gif)

4. You should now be able to see your new files in your repository in your GitHub account

### Hosting on GitHub Pages

#### Why GitHub Pages?

Etters (2016) says, "\[h]osting your content on a website gives you the power to fix inaccuracies almost instantly and keep your content in sync with the latest software release". A great example of a hosting site is GitHub Pages. GitHub Pages is available for GitHub users and enables them to host their static websites. We are using this to host our static website because it pairs well with our GitHub version control since they are both on the same site. GitHub Pages also has a built in Jekyll static site generator which makes choosing a theme easy. I recommend using GitHub Pages as it seamlessly integrates with other components of our software stack.

#### Instructions

1. Navigate to the __Settings__ tab in your repository
2. Then click the __Pages__ tab on the left navigation bar
3. Within the __Pages/GitHub Pages__ tab, under the __Source__ section, set the source to be __master/root__ or __main/root__, depending on how your GitHub is configured
4. Next press __Save__ for the __Source__ section
5. You may now view your static site at __https://\<username\>.github.io__
    * For example, if my username was JohnDoe then my static site will be published at  __https://johndoe.github.io/__

### Choosing your Jekyll theme

#### Why Jekyll?
Jekyll is a static site generator that processes lightweight markup languages like Markdown and a theme, into "beautiful \[and] functional website\[s]" (Etter, 2016, p. 26). Furthermore, static site generators are great to use because they have "no server-side application dependencies, no databases, and nothing to install, so migrating the entire site is as easy as moving a directory" (Etter, 2016, p. 26). Also, static websites are testable on your local computer without the need of any additional installations or having to "compress and ship them with software applications" (Etter, 2016, p. 26). It is possible to create simple static websites manually, but to make things easier and "to do anything complex, you'll want to use a generator" (Etter, 2016, p. 26).

#### Instructions

1. Navigate to the __Settings__ tab in your repository
2. Then click the __Pages__ tab on the left navigation bar
3. Within the __Pages/GitHub Pages__ tab, under __Theme chooser__, click the __Change theme__ button.
4. Explore your theme options and once you have settled on your favorite, click the __Select theme__ button
5. View the Jekyll theme applied to your static site at __https://\<username\>.github.io__
    * For example, if my username was JohnDoe then my static site will be published at  __https://johndoe.github.io/__

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

1. “Why is Markdown better than a word processor?”
    __Answer:__ "Documentation with any sort of lifespan needs to be kept in version control" (Etter, 2016, p. 20). Markdown is better than word processors when it comes to creating documentation. Word processors create PDFs that can be consumed and discarded. Therefore, for creating documentation, Markdown is better than a word processor because it can used with version control. This makes Markdown documentation easy to edit and update for future versions. 
2. "Why is my theme not rendering on my static website?" 
    __Solution 1:__ It may take a while for your changes to apply to the static website, wait 5-10 minutes and check back again. 
    __Solution 2:__ Additionally, clear your browser's cache and refresh the page, then your theme may show.

