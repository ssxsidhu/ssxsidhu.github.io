# Hosting a Resume with Markdown, VS Code, GitHub Pages, and Jekyll

## Purpose

This README's goal is to outline the detailed procedures for hosting and formatting a résumé using Markdown, VS Code, GitHub Pages, and Jekyll. The general guidelines of contemporary technical writing, as outlined in Andrew Etter's book Modern Technical Writing, will also be related to these practical processes.

## Prerequisites

You'll need a résumé that is Markdown-formatted before you can proceed with the guidelines below. We suggest starting with a [Markdown tutorial](https://www.markdowntutorial.com/) if you are new to Markdown.

## Instructions

### 1\. Create a New Project Folder in VS Code

First, open VS Code and create a new folder for your website project. You can do this by going to `File` > `Open Folder` and selecting a new empty folder.

### 2\. Create an `index.md` File

Next, create a new file in the folder and name it `index.md`. This file will serve as the main page of your website.

### 3\. Copy Your Resume into `index.md`

Open your Markdown resume file in a separate tab in VS Code. Copy the contents of your Markdown resume file into `index.md`.

### 4\. Add Front Matter to `index.md`

Add front matter to `index.md` to specify the layout and metadata for your website. Front matter is a YAML block that appears at the beginning of your file and tells Jekyll how to handle the file. Here is an example:

```
---
layout: default
title: [Your Name] - Resume
--- 
```

The `layout` parameter specifies the layout to use for the page, and the `title` parameter specifies the title of the page, which will appear in the browser tab and search results.

### 5\. Save `index.md`

Save `index.md` to ensure that your changes are preserved.

### 6\. Install Jekyll

Install Jekyll by following the [official installation guide](https://jekyllrb.com/docs/installation/). This will install all the necessary components and dependencies to run your website.

### 7\. Create a New Jekyll Site

Create a new Jekyll site in your project folder by running 
```
jekyll new .
``` 
in the terminal. This will create all the necessary files and folders for a basic Jekyll site.

### 8\. Serve Your Website

Run `bundle exec jekyll serve` in the terminal to build and serve your website. This will generate your site and make it available at `http://localhost:4000`.

```
bundle exec jekyll serve
```

### 9\. Preview Your Website

Open your web browser and go to `http://localhost:4000` to view your website. This is a good opportunity to check that your website is working as expected.

### 10\. Commit and Push Your Changes
Commit and push your changes to a GitHub repository or a Codeberg repository. This will ensure that your website is available to the world.


```
git add.
git commit -m "Add resume to website"
git push origin main
```

### 11\. Enable GitHub Pages or Codeberg Pages

Go to your repository settings and enable GitHub Pages or Codeberg Pages, choosing the `main` branch as the source. This will make your website available online.

### 12\. Check Your Website

Your website should now be accessible at `https://[your-username].github.io/[repository-name]/` or `https://[your-username].codeberg.page/[repository-name]/`. Check your website to make sure it is working as expected.

### Customizing Your Website

To make your website more visually appealing, you can customize the Jekyll theme by editing the `_config.yml` file and the HTML and CSS files in the `_layouts` and `_includes` folders. You can also add more pages and content to your website by creating

## Relating to Technical Writing Principles

1. Utilize Lightweight Markup Languages: Etter advocates creating technical documentation using lightweight markup languages such as Markdown. This approach is followed by utilising Markdown to format your resume.

2. Automate Documentation Tasks: Etter also suggests using technologies like Jekyll to automate documentation chores. This idea is followed by utilising Jekyll to convert your Markdown file to HTML and host your website.
3. Web-Publish Documents: Etter proposes making documents available on the web in order to reach a larger audience. You can host your CV on GitHub Pages or Codeberg.

## More Resources

1. [Markdown tutorial](https://www.markdowntutorial.com/)
2. [Modern Technical Writing by Andrew Etter](https://www.amazon.com/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS)
3. [Jekyll documentation](https://jekyllrb.com/docs/)

## Authors and Acknowledgments

This README was written by Sahilpreet.
Also, the author would like to acknowledge his teammates (Group 16) :

- Jasmine Tabuzo 
- Eric Shu 
- Kha Pham 

## FAQs

### Why is Markdown better than a word processor?

It's simple to learn and utilise the lightweight markup language known as markdown. It enables plain text formatting, which is quicker and more effective than using a word processor. Moreover, Markdown generates clear, clean HTML code, making it simpler to convert your content to other forms like PDF or HTML.

### Why is my resume not showing up?

There could be a few reasons why your CV does not appear on your website. To begin with, confirm that your resume file is saved in the appropriate place and has the appropriate name. Second, check that your resume file's front matter is properly formatted. Finally ,confirm that your website is being delivered correctly and that your Jekyll configuration file is configured appropriately. If you are still having problems, look for answers in Jekyll's documentation or get support from internet forums.
