[![Netlify Status](https://api.netlify.com/api/v1/badges/28fd98db-efdc-4457-889c-9521ee0f686e/deploy-status)](https://app.netlify.com/sites/hugo-in-wonderland/deploys)
# Example Site for webcomic theme
I'm using this repo to develop a hugo theme for webcomics. It has also been set up to use [Netlify](https://www.netlifycms.org/) for free deployment and content management. Basically, it's a ready-to-use webcomic site. Just add comics!

## Features
- Pre-configured Netlify admin page for easy content management
- Graphic header with configurable links
  - [Bulma classes](https://bulma.io/documentation/overview/classes/) can be added to the header via the hugo config.toml to change the appearance.
- Sticky footer with configurable links
- Full-size comic display with navigation buttons
- Comic archive page which can be further divided into chapters
- Configurable 'About' page
- Flexible posts that can be used as additional info pages or as a traditional blog

## Local Development
Make sure you have the latest version of the theme in the submodule:
```bash
$ cd themes/webcomic-theme
$ git pull origin master
```

Then use hugo to serve the site locally:
```bash
$ hugo serve
```

## Deploy with Netlify
This repo has the necessary configuratin and static pages to use Netlify content management system. The files that configure and display Netlify's content management system are located in `static/admin`. To deploy your own copy of this repo:
1. Fork this repo.
2. Create a free Netlify account and follow Netlify's instructions [here](https://www.netlifycms.org/docs/hugo/#deploying-with-netlify) to deploy. 

## Style
### Header Graphic
Replace `banner.jpg` with your own image to change the graphic header image. Bigger is better! The top left corner of the header image will be aligned with the top left corner of your user's screen. How much of the image viewers see depends on the device they're using. The example header comes from [Masaaki Komori on Unsplash](https://unsplash.com/photos/qgEKJkf4sKY). 

## Background Image
replace `background.png` with your own image to change the background. I chose a [tile-able image from toptal subtle patterns](https://www.toptal.com/designers/subtlepatterns/handmade-paper/) for the example. If you want to use a larger non-tiled background, you'll have to mess with the css a bit. I recommend this for a large, fixed background (tip from [css tricks](https://css-tricks.com/perfect-full-page-background-image/)):
```css
html { 
  background: url(images/bg.png) no-repeat center center fixed; 
  -webkit-background-size: cover;
  -moz-background-size: cover;
  -o-background-size: cover;
  background-size: cover;
}
```
