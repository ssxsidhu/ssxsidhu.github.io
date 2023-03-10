![1](resume.gif)

# Hosting a Resume with Markdown, VS Code, GitHub Pages, and Jekyll

## Purpose

This README's goal is to outline the detailed procedures for hosting and formatting a resume using Markdown, VS Code, GitHub Pages, and Jekyll. The general guidelines of contemporary technical writing, as outlined in Andrew Etter's book Modern Technical Writing, will also be related to these practical processes.

## Prerequisites

- You'll need a resume that is Markdown-formatted before you can proceed with the guidelines below. If you are new to Markdown, we suggest starting with a Markdown tutorial, a link for which can be found in [more resources section](#more-resources).
- [Git](https://git-scm.com/downloads)
- [VS Code](https://code.visualstudio.com/download)

## Instructions

### Step 1: Create a new repository on GitHub

1. Log in to your GitHub account.
2. Click on the "+" icon in the top right corner and select "New repository".
3. Name your repository `<username>.github.io`, where `<username>` is your GitHub username.
4. Select "Public" for the repository visibility.
5. Click on "Create repository".

### Step 2: Enable GitHub Pages

1. In your GitHub repository, click on the "Settings" tab.
2. Scroll down to the "GitHub Pages" section.
3. Under "Source", select "main" from the dropdown menu and click on "Save".
4. You should see a message that says "Your site is ready to be published at `<username>.github.io`".

### Step 3: Clone the repository to your local machine

1. Open VS Code.
2. Press `Ctrl+Shift+P` (Windows) or `Cmd+Shift+P` (Mac) to open the Command Palette.
3. Type "Git: Clone" and press Enter.
4. Paste the URL of your GitHub repository (e.g., `https://github.com/<username>/<username>.github.io.git`) and press Enter.
5. Select a location on your local machine where you want to save the repository.

### Step 4: Install Jekyll

1. Install Jekyll by following the [official installation guide](https://jekyllrb.com/docs/installation/).
2. This will install all the necessary components and dependencies to run your website.

### Step 5: Create a new Jekyll site

1. In VS Code, open the terminal (`Ctrl+` \` (Windows) or `Cmd+` \`  (Mac)).
2. Navigate to your cloned repository folder using the `cd` command.
3. Create a new Jekyll site in your project folder by running `jekyll new .`
4. This will create all the necessary files and folders for a basic Jekyll site.

### Step 6: Set up your project

1. Open your Markdown resume file in a separate tab in VS Code.
2. Open the newly created `index.markdown` 
3. Don't remove the front matter in `index.markdown` as it is used to specify the layout and metadata for your website.
4. Copy the contents of your Markdown resume file into `index.markdown`.
5. Save `index.markdown` to ensure that your changes are preserved.

## Step 7: Preview your resume

1. In VS Code, press `Ctrl+Shift+V` (Windows) or `Cmd+Shift+V` (Mac) to open the Markdown preview window.
2. You should see a preview of what your resume will look like when it's rendered as HTML.

### Step 8: Serve and preview your website

1. In the terminal, run `bundle exec jekyll serve` to build and serve your website.
2. This will generate your site and make it available at `http://localhost:4000`.
3. Open your web browser and go to `http://localhost:4000` to view your website.
4. This is a good opportunity to check that your website is working as expected.

### Step 9: Commit and push changes

1. In VS Code, press `Ctrl+Shift+G` (Windows) or `Cmd+Shift+G` (Mac) to open the Source Control panel.
2. Stage all changes by clicking on "+" next to each file in the list of changes.
3. Enter a commit message (e.g., "Add initial version of resume") in the text field at the top of the panel.
4. Press `Ctrl+Enter` (Windows) or `Cmd+Enter` (Mac) to commit changes.
5. Click on the "..." icon in the top right corner of the Source Control panel and select "Push" to push changes to GitHub.
6. Wait a few minutes for GitHub Pages to build your site with Jekyll.
7. Refresh `<username>.github.io` in your web browser to see your customized resume.

That's it! You have successfully hosted and formatted a resume using Markdown, VS Code, GitHub Pages and Jekyll.

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
