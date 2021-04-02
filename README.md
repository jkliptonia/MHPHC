# MHPHC Newsletter Site

To begin to use this project, pull down the repo and run `npm install`.  This will install 11ty and all other tools required.  

Run `npm build` and 11ty will process your changes to the rendered site files.  You can run `npm start` and 11ty will serve your site locally.  You can click on the `http://localhost:3001` link to see the site in your browser.

To publish your changes, you will need to follow the deployment instructions below.

## Table of Contents

1. [Intro](#intro)
2. [Making Changes](#making-changes)
3. [Troubleshooting](#troubleshooting)
4. [Resources](#resources)
5. [Misc Info](#misc-info)

## Intro

You currently only have two pages to worry about, they are `index.md` and `404.md`.  As you can probably guess, `404.md` is just your "file not found" page, in case a link breaks, so *really* you only need to worry about `index.md`.  Any folders that start with an "_" you should not edit.

These files are written in a language called Markdown, which is really just a shortcut to HTML.  Want a < h1 >?  Use a single `#`.  Two `#`s gets you an < h2 >.  My hope is that this will be easier to work with, and make sharing the project easier if you'd like to pass this off someday.

Here is a full [Markdown cheatsheet](https://www.markdownguide.org/cheat-sheet/) which should have everything you need.  The top section of the file is for your template, which you shouldn't need to worry about.  If you ever do though, it's HTML with help from a templating language called [Liquid](https://shopify.github.io/liquid/basics/introduction/).

Markdown also understands basic html, so if you get sick of it, you can always throw a `< bold >` in there if you feel the need.

## Making Changes
Making changes should be easy.  You can change any copy in any of the `.md` files (see cheatsheet in resources) under the top section.  You can also edit things in the top section as long as you don't remove any of the specific categories (excluding the layout).

To add a new newsletter, add it to the `/archive` folder and make sure it is named accordingly.  Then, add it to the list in `index.md`.

After any changes, you need to run `npm build`.  This will trigger 11ty to process your changes and produce new site files ready to be deployed.  

You can check out your changes by running `npm start`.  11ty will do some voodoo, and then you will see a link in your terminal which you can `CMD + Click` to load the site in your browser.

When you are satisfied with your changes, you need to save your changes to Github, which is the code repository we're using.  Run `git add .` and then `git commit -m "[insert whatever message you'd like]"`.  This essentially creates a save of your work.  You can then store these changes to Github by running `git push origin mother` and the internet will save your changes, but not yet publish them to the site.

The final step is to deploy your changes.  This will publish them to the live website.


## Troubleshooting

### Editing

### Saving

### Deploying

## Resources

- [Markdown cheatsheet](https://www.markdownguide.org/cheat-sheet/)

## Misc Info

Just in case you ever need to know, this website is built with Markdown (text-to-html converting language), [11ty](https://www.11ty.dev/) (site generating utility), and [Node.js](https://nodejs.org/en/) (a javscript based runtime environment), and deployed on [Netlify](https://www.netlify.com/) (a free hosting platform).