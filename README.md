# GitHub Pages

_Create a site or blog from your GitHub repositories with GitHub Pages._


With GitHub Pages, you can host project blogs, documentation, resumes, portfolios, or any other static content you'd like. Your GitHub repository can easily become its own website. In this course, we'll show you how to set up your own site or blog using GitHub Pages.

- **Who is this for**: Beginners, students, project maintainers, small businesses.
- **What you'll learn**: How to build a GitHub Pages site.
- **What you'll build**: We'll build a simple GitHub Pages site with a blog. We'll use [Jekyll](https://jekyllrb.com), a static site generator.
- **How long**: This course is five steps long and takes less than one hour to complete.

## How to start this course

1. Open following URL in browser, click **Fork** and open the link in a new tab.
   `https://github.com/fenago/github-pages`

   ![](./images/1.jpg)
2. In the new tab, follow the prompts to create a new repository.
   - For owner, choose your personal account or an organization to host the repository.
   - We recommend creating a public repository—private repositories will [use Actions minutes].
    ![](./images/2.jpg)
3. After your new repository is created, wait about 20 seconds, then refresh the page. Follow the step-by-step instructions in the new repository's README.


<summary><h2>Step 1: Enable GitHub Pages</h2></summary>

_Welcome to GitHub Pages and Jekyll :tada:!_

The first step is to enable GitHub Pages on this [repository]. When you enable GitHub Pages on a repository, GitHub takes the content that's on the main branch and publishes a website based on its contents.

### Activity: Enable GitHub Pages

1. Open a new browser tab, and work on the steps in your second tab while you read the instructions in this tab.
1. Under your repository name, click **Settings**.
1. Click **Pages**, in the "GitHub Pages" section, use the Source drop-down, then select **main branch**.
1. Wait about _one minute_, then refresh this page for the next step.
   > Turning on GitHub Pages creates a deployment of your repository. GitHub Actions may take up to a minute to respond while waiting for the deployment. Future steps will be about 20 seconds; this step is slower.


<summary><h2>Step 2: Configure your site</h2></summary>

_You turned on GitHub Pages! :tada:_

We'll work in a branch, `my-pages`, that I created for you to get this site looking great. :sparkle:

Jekyll uses a file titled `_config.yml` to store settings for your site, your theme, and reusable content like your site title and GitHub handle. You can check out the `_config.yml` file on the **Code** tab of your repository.

We need to use a blog-ready theme. For this activity, we will use a theme named "minima".

### Activity: Configure your site

1. Browse to the `_config.yml` file in the `my-pages` branch.
1. In the upper right corner, open the file editor.
1. Add a `theme:` set to **minima** so it shows in the `_config.yml` file as below:
    ```yml
    theme: minima
    ```
1. (optional) You can modify the other configuration variables such as `title:`, `author:`, and `description:` to further customize your site.
1. Commit your changes.
1. Wait about 20 seconds then refresh this page for the next step.


<summary><h2>Step 3: Customize your homepage</h2></summary>

_Nice work setting the theme! :sparkles:_

You can customize your homepage by adding content to either an `index.md` file or the `README.md` file. GitHub Pages first looks for an `index.md` file. Your repository has an `index.md` file so we can update it to include your personalized content.

### Activity: Create your homepage

1. Browse to the `index.md` file in the `my-pages` branch.
1. In the upper right corner, open the file editor.
1. Type the content you want on your homepage. You can use Markdown formatting on this page.
1. (optional) You can also modify `title:` or just ignore it for now. We'll discuss it in the next step.
1. Commit your changes to the `my-pages` branch.
1. Wait about 20 seconds then refresh this page for the next step.


<summary><h2>Step 4: Create a blog post</h2></summary>

_Your home page is looking great! :cowboy_hat_face:_

GitHub Pages uses Jekyll. In Jekyll, we can create a blog by using specially named files and frontmatter. The files must be named `_posts/YYYY-MM-DD-title.md`. You must also include `title` and `date` in your frontmatter.

**What is _frontmatter_?**: The syntax Jekyll files use is called YAML frontmatter. It goes at the top of your file and looks something like this:

```yml
---
title: "Welcome to my blog"
date: 2019-01-20
---
```

For more information about configuring front matter, see the [Jekyll frontmatter documentation](https://jekyllrb.com/docs/frontmatter/).

### Activity: Create a blog post

1. Browse to the `my-pages` branch.
1. Click the `Add file` dropdown menu and then on `Create new file`.
1. Name the file `_posts/YYYY-MM-DD-title.md`.
1. Replace the `YYYY-MM-DD` with today's date, and change the `title` of your first blog post if you'd like.
   > If you do edit the title, make sure there are hyphens between your words.
   > If your blog post date doesn't follow the correct date convention, you'll receive an error and your site won't build. For more information, see "[Page build failed: Invalid post date]".
1. Type the following content at the top of your blog post:
   ```yaml
   ---
   title: "YOUR-TITLE"
   date: YYYY-MM-DD
   ---
   ```
1. Replace `YOUR-TITLE` with the title for your blog post.
1. Replace `YYYY-MM-DD` with today's date.
1. Type a quick draft of your blog post. Remember, you can always edit it later.
1. Commit your changes to your branch.
1. Wait about 20 seconds then refresh this page for the next step.


<summary><h2>Step 5: Merge your pull request</h2></summary>

_Nice work, friend :heart:! People will be reading your blog in no time!_

You can now [merge] your pull request!

### Activity: Merge your pull request

1. Click **Merge pull request**.
1. Delete the branch `my-pages` (optional).
1. Wait about 20 seconds then refresh this page for the next step.




<summary><h2>Finish</h2></summary>

_Congratulations friend, you've completed this course!_

Your blog is now live and has been deployed!

Here's a recap of all the tasks you've accomplished in your repository:

- You enabled GitHub Pages.
- You selected a theme using the config file.
- You learned about proper directory format and file naming conventions in Jekyll.
- You created your first a blog post with Jekyll!
