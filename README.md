This guide shows you how to create [a simple website](https://matcttu.github.io/) on GitHub pages for free. The website is a fork of the Jekyll theme **[Moon](https://taylantatli.github.io/Moon)**. You can browse other free themes at [jekyllthemes.io/free](https://jekyllthemes.io/free).

This guide is not an introduction to Git nor any best practices.

## Getting Started

1. [Create a GitHub account](https://github.com/join).

   > Note that the username you choose will be a part of your web address.

   Make sure you verify the confirmation email.
   
   ![Verify conformation email](https://i.imgur.com/NIGYlVK.gif)

1. Click **Fork** at the top of this page to make a copy of the `matcttu.github.io` repository.

   ![Click fork](https://i.imgur.com/sqL26aO.gif)

   After a few moments, all of the files will be copied into a repository you own.

1. Click **Settings**.

   ![Click settings](https://i.imgur.com/Z3rzO7t.gif)

1. Replace `matcttu` with your username, and then click **Rename**.

   ![Update the Repo name](https://i.imgur.com/RV0kw0A.gif)

   > Note that `**username**.githib.io` will be your site's URL or web address, but before you can visit your site, you need to update the config file.

1. Click `_config.yml` to open the file.

   ![Open _config.yml](https://i.imgur.com/hsthdhY.gif)

    This config file controls many aspects of the site including front page text, logo and background branding, and social icons, but you can ignore all of that for right now.

1. Click the Pencil icon to open the file for editing and then replace `MATCTTU` on line 11 with your username.

   ![Click the pencil icon](https://i.imgur.com/g1hJqNC.gif)

1. Scroll all the way down, then click **Commit changes**.

   ![Commit changes](https://i.imgur.com/jP06v9A.gif)

   > Note that commiting changes directly to the `master` branch and without descriptions is in fact a **BAD** practice. Avoid this in actual colaborative projects.

You can now view your live site at https://username.github.io, replacing `username` with your username, of course. If you don't see your site, go to **Settings** > **Pages** to verify GitHub Pages is publishing your site. You also may have to change the Source branch:

![Change source branch](https://i.imgur.com/VF2CRmm.gif)

## Customizing your site

### The home page

1. Reopen `_config.yml` and click the pencil icon

1. Replace `My MATC Portfolio` on line 2 with a new title for your site.

1. Replace `This is a description of this site.` on line 3 with a new description for your site.

1. Replace `My portfolio in partial fullfillment of Texas Tech's MATC.` on line 4 with a new description. Note that while this text doesn't appear on the page, it affects SEO and will be displayed in search engine results.

1. Click **Commit changes** to publish your changes. Note that it may take up to 10 minutes for your changes to rollout.

#### Branding

Lines 7 and 8 of the `_config.yml` show you that the logo and background images are named `logo.png` and `placeholder-big.jpg`. It's quickest to leave `_config.yml` alone and upload new images with the same names to the images folder.

1. From the main repo page click **assets**, and then click **img** to open the images folder.

1. Click **Add a file**, and then click **Upload files**.

1. Drag and drop the images you want to upload, and then click **Commit changes**. Note that it may take up to 10 minutes for your changes to rollout.

   > Note that files with the same names will be replaced. If you uploaded files with different images, edit lines 7 and 8 in the `_config.yml` file to reflect the new names.

#### Social icons

1. Reopen `_config.yml` and click the pencil icon
   
   Lines 33 through 63 list the built-in social icons.

1. Add a `#` at the beginning of any line to remove an icon.

1. Delete the `#` at the beginning of any line and replplace `username` with your social media's username to add an icon.

1. Click **Commit changes** to publish your changes. Note that it may take up to 10 minutes for your changes to rollout.

### The about page

1. From the main repo page click **about**, and then click **index.md** to open the about page.
1. Click the Pencil icon to edit the page.
1. Tailor the page to you, and then click **Commit changes**. Note that it may take up to 10 minutes for your changes to rollout.

### Adding posts and projects

Posts and projects both live in the `_posts` folder. The only difference is that projects have the line `project: true` in the front matter. The front matter is everything between the ---s at the beginning of the file.

For new projects, use the following template:

```
---
layout: post
title:  "Put your title here"
date:   2021-04-31
excerpt: "This is a short description that should entice readers to want to read the full text."
project: true
tag:
- keyword
- other keyword
- etc...
feature: https://i.imgur.com/fU0XhVE.jpg
comments: true
---
```

1. From the main repo page click **_posts**

1. Click **Add a file**, and then click **Create a file**.

1. Enter the name of your project in the following format `year-month-day-project-title.md`, for example `2021-04-31-my-first-post.md`

   > Note that everything following the day will be make up the posts URL, so keep it short.

1. Copy and paste the template from above into the file.

1. Customize the front matter. Additionally, you may
    - Delete `project: true` to create a new post.
    - Replace the link in `feature: https://i.imgur.com/fU0XhVE.jpg` with a link or path to the image you want to use.
    - Delete the `feature: https://i.imgur.com/fU0XhVE.jpg` line to create a project or post without an image.

1. Write your post, and then click **Commit changes**. Note that it may take up to 10 minutes for your changes to rollout.

### Deleting posts and projects

1. From the main repo page click **_posts**

1. Click the file you want to delete.

1. Click the Trashcan icon.

1. Scroll all the way down, and then click **Commit changes**. Note that it may take up to 10 minutes for your changes to rollout.
