# Example Site for webcomic theme
I'm using this repo to develop a hugo theme for webcomics. It has also been set up to use [Netlify](https://www.netlifycms.org/) for free deployment and content management. Basically, it's a ready-to-deploy webcomic site. Just add comics!

## Local Development
Make sure you have the latest version of the theme in the submodule:
```bash
$ cd themes/webcomic theme
$ git pull origin master
```

Then use hugo to serve the site locally:
```bash
$ hugo serve
```

## Deploy with Netlify
Fork this repo, create a free Netlify account, and follow Netlify's instructions [here](https://www.netlifycms.org/docs/hugo/#deploying-with-netlify) to deploy. The files that configure and display Netlify's content management system are located in `static/admin`.