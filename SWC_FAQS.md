# SWC Frequently Asked Questions

##### Set Up
- [How do you properly install your theme?](#InstallTheme)
- [The comic pagination is not showing up](#ComicPagination)
- [The comic pagination buttons are appearing very small](#ComicPaginationSmall)
- [Is there a way to add a link to my first comic page in the navigation bar?](#PageLink)
- [How do I show the “Ask” link?](#AskLink)

##### Trouble Shooting
- [The “First” button is going to the wrong page](#FirstButtonURL)
- [My “First” button has disappeared](#FirstButtonDisappeared)
- [I can't see my share buttons](#ShowShareButtons)
- [My banner image is not showing](#ShowBannerImage)
- [My Google+ link is not going to the correct URL](#GoogleLink)
- [My “Show Social Links” is on, but I can't see the logo (picture) of each social links](#SocialLinksColours)
- [Why does my Google Analytics status say “Tracking code not verified”?](#GoogleAnalyticsStatus)

##### Design
- [Is there a way for the header and aside to have a transparent background?](#TransparentHeader)
- [How can I center the navigation links?](#CenterNavigation)
- [How do I get rid of the shadow under the navigation?](#NavigationShadows)
- [How do I reduce the space above and below the comic pagination?](#ComicPaginationSpace)
- [How do I reduce the top padding in the content area?](#ContentTopPadding)
- [How do I increase the content width?](#ContentWidth)
- [Is there a way to make post show in chronological order?](#ChronologicalOrder)
- [Is there a way to add Disqus on the homepage?](#Disqus)
- [How can I have the images width on my custom page the same as the wrapper width?](#PageImageWidth)
- [How do I change the clicked-link colour?](#VisitedLinkColour)
- [How can I enlarge the post author portrait in Simple Webcomic to make it bigger than 24x24?](#PostAvatarSize)
- [Is there a way to make the “About” section in the footer wider?](#WiderFooterSection)

---

###### Set Up

<a name="InstallTheme">
###How do you properly install your theme?
First, start by going to: [https://www.tumblr.com/theme/39018](https://www.tumblr.com/theme/39018)

Click the "Install" button and select the blog you would like the theme to be installed on.

With the theme installed, converting your Tumblr blog to a webcomic can be achieved in just two simple steps:

1. In the theme options, you will need to turn on “Comic Pagination”.
2. Scroll down and click on “Advance options”, set “Posts per page” to 1.

*Once you have published your first post you should copy and paste the post permalink into the "First Post URL" field. This ensures the comic pagination works correctly.*

Optional:
- To make your post image link to the next page, turn on "Clickable images".
- To include a random page link, turn on "Random button".

You can find a full breakdown of all the options here: [https://github.com/geoneo1/SimpleWebcomicTheme/blob/master/SWC_THEME_OPTIONS.md] (https://github.com/geoneo1/SimpleWebcomicTheme/blob/master/SWC_THEME_OPTIONS.md)

<a name="ComicPagination">
### The comic pagination is not showing up
In order for the comic pagination to appear, you need to have more than one post. I suggest having three posts to test all four of the buttons. 

<a name="ComicPaginationSmall">
### The comic pagination buttons are appearing very small
You can increase the height of your comic pagination images by changing the number in the "Comic pagination image height" field. The default is 24(px). Once you increase that, they will display larger.

<a name="PageLink">
### Is there a way to add a link to my first comic page in the navigation bar? 
1. Go to the Edit theme area
2. Scroll all the way down to the bottom and click “Add a Page” button
3. Click on the “Standard Layout” dropdown and select “Redirect”
4. Click the “Show a link to this page” toggle button
5. Once that is on you will be able to name your link
6. In the first field you can choose a custom URL
8. Then in the “Redirect to” field paste the URL of your first comic page

<a name="AskLink">
### How do I show the “Ask” link?
The theme does have an ask feature, but the setting is hidden away in the general tumblr options. 

In your tumblr dashboard, in the top right you should see a user icon (next to the lightning bolt). Click on that and select “Edit appearance”. The 4th option down is “Ask”, Make sure “Let people ask questions” is activated. Once it is, the link should appear in the theme automatically.

---

###### Trouble Shooting

<a name="FirstButtonURL">
###The “First” button is going to the wrong page
You must add the *post URL* in the “First comic page URL” field, not the *page URL*.

Go to your first comic page and click on either the date or the the link icon. Then just copy the URL and paste it into the "First comic page URL" field. Then save.

<a name="FirstButtonDisappeared">
### My “First” button has disappeared
Shortly after launching the theme a user bought to my attention that the first blog post may not necessarily be the first comic page. So I implemented a theme change to factor that in. 

Originally, as long as you had more than one post, the “First” button would show up, regardless if you filled in “First post URL” or not. Now, you *have to include the post URL* of your first comic page in the theme field “First comic page URL” in order for the “First” button to appear. 

Furthermore, as I changed the field name from “First post URL” to “First comic page URL” Tumblr treats it as a completely new field. The data you may have already entered is cleared requiring you to put it in again. 

<a name="ShowShareButtons">
### I can't see my share buttons
Make sure that the “Post metadata" option is turned on. The Post metadata includes the *author*, *time stamp*, *tags*, *notes*, *comment count*, *content source*, as well as all the *share options*. The theme has options to individually hide these features.

<a name="ShowBannerImage">
### My banner image is not showing
1. Go to the Edit theme area 
2. Make sure “Show header image" is on

If you are using one large image:

- Make sure “Repeat header” image is off
- You can adjust "Header height” option to better suit your image

*Note: If you are using “Big header” It will override the Header height option.*

<a name="GoogleLink">
### My Google+ link is not going to the correct URL
For “Google Plus Username” to work you will require a *Google+ Custom URL*. Please take a look at [Getting Started with Google+ Custom URLs] (http://goo.gl/9oRRRH).

<a name="SocialLinksColours">
### My “Show social links” is on, but I can't see the logo (picture) of each social links

The background of the social links are determined your “Accent color”, the icons are determined by your “Aside text” colour, if these two are the same colour, you will not be able to see the icons. However, you can change the colour of the background. 

Go to the Edit theme area, scroll to the bottom and click “Advanced options”, then copy and paste the following into the “Add custom CSS” field:
```
.social-links ul li a span.ico { background-color: #222; }
```
If you prefer to keep the background as is and change the icon colour instead, paste this:
```
.social-links ul li a { color: #fff; }
```

<a name="GoogleAnalyticsStatus">
### Why does my Google Analytics status read “Tracking code not verified”?
After adding the your Google Analytics tracking code in your theme options, it may take 24 hours for data to appear in your reports.

---

###### Design

<a name="TransparentHeader">
### Is there a way for the header and aside to have a transparent background?
Go to the Edit theme area, scroll to the bottom and click “Advanced options”, then copy and paste the following into the “Add custom CSS” field:
```
header#masthead, .alternative aside, .alternative footer.sub-basement { background-color: transparent; }
```
This removes the shadow from the Header (should you want to):
```
header#masthead > div { box-shadow: none; }
```

<a name="CenterNavigation">
### How can I center the navigation links?
Go to the Edit theme area, scroll to the bottom and click “Advanced options”, then copy and paste the following into the “Add custom CSS” field:
```
nav#access .wrapper { text-align: center; }
```

<a name="NavigationShadow">
### How do I get rid of the shadow under the navigation?
Go to the Edit theme area, scroll to the bottom and click “Advanced options”, then copy and paste the following into the “Add custom CSS” field:
```
nav#access { box-shadow: none !important; }
```

<a name="ComicPaginationSpace">
### How do I reduce the space above and below the comic pagination?
Go to the Edit theme area, scroll to the bottom and click “Advanced options”, then copy and paste the following into the “Add custom CSS” field:
```
.comic-pagination, .pagination { padding: 2em 0 0; }
footer.metadata { margin-top: 2em; }
```
In this case 2em equals 32px. I am using ems, you can use pxs if you are more comfortable with the. 

<a name="ContentTopPadding">
### How do I reduce the top padding in the content area?
Go to the Edit theme area, scroll to the bottom and click “Advanced options”, then copy and paste the following into the “Add custom CSS” field:
```
article { padding-top: 2em; }
```
*The default is 4em (which is 64px), in the example I have halved it, but you can change it to whatever suits you. You don't need to stick to ems either, you can use px if you prefer.*

<a name="ContentWidth">
### How do I increase the content width?
Go to the Edit theme area, scroll to the bottom and click “Advanced options”, then copy and paste the following into the “Add custom CSS” field:
```
article > *, div#disqus_thread, section#notes,
.alternative article > *, .alternative div#disqus_thread, .alternative section#notes {
  width: 80%;
}

@media only screen and (max-width:480px){
  article > *, div#disqus_thread, section#notes,
  .alternative article > *, .alternative div#disqus_thread, .alternative section#notes {
    width:90%
  }
}
```

<a name="ChronologicalOrder">
### Is there a way to make post show in chronological order?
I did look into adding this feature when I was building the theme, but as far as I am aware, tumblr does not allow theme builders this feature.

There is a way you can do it using tags  http://staff.tumblr.com/post/34933619/new-feature-tag-filtering

I usually advise people to create “Read from the beginning” link in the main nav that links to the first comic page URL. 

<a name="Disqus">
### Is there a way to add Disqus on the homepage?
Disqus comments only appear on the individual posts because they require a unique URL. If they were to appear on the homepage, when you add a new post, any previous comments will still be visible. Which may result in unrelated comments. 

If you still want it to appear on the homepage, there is a way but it would mean the comments will show on all pages, including any custom pages. 

If you still would like to add comments to pages: 

1. Go to the Edit theme area# SWC Frequently Asked Questions

##### Set Up
- [How do you properly install your theme?](#InstallTheme)
- [The comic pagination is not showing up](#ComicPagination)
- [The comic pagination buttons are appearing very small](#ComicPaginationSmall)
- [Is there a way to add a link to my first comic page in the navigation bar?](#PageLink)
- [How do I show the “Ask” link?](#AskLink)

##### Trouble Shooting
- [The “First” button is going to the wrong page](#FirstButtonURL)
- [My “First” button has disappeared](#FirstButtonDisappeared)
- [I can't see my share buttons](#ShowShareButtons)
- [My banner image is not showing](#ShowBannerImage)
- [My Google+ link is not going to the correct URL](#GoogleLink)
- [My “Show Social Links” is on, but I can't see the logo (picture) of each social links](#SocialLinksColours)
- [Why does my Google Analytics status say “Tracking code not verified”?](#GoogleAnalyticsStatus)

##### Design
- [Is there a way for the header and aside to have a transparent background?](#TransparentHeader)
- [How can I center the navigation links?](#CenterNavigation)
- [How do I get rid of the shadow under the navigation?](#NavigationShadows)
- [How do I reduce the space above and below the comic pagination?](#ComicPaginationSpace)
- [How do I reduce the top padding in the content area?](#ContentTopPadding)
- [How do I increase the content width?](#ContentWidth)
- [Is there a way to make post show in chronological order?](#ChronologicalOrder)
- [Is there a way to add Disqus on the homepage?](#Disqus)
- [How can I have the images width on my custom page the same as the wrapper width?](#PageImageWidth)
- [How do I change the clicked-link colour?](#VisitedLinkColour)
- [How can I enlarge the post author portrait in Simple Webcomic to make it bigger than 24x24?](#PostAvatarSize)
- [Is there a way to make the “About” section in the footer wider?](#WiderFooterSection)

---

###### Set Up

<a name="InstallTheme">
###How do you properly install your theme?
First, start by going to: [https://www.tumblr.com/theme/39018](https://www.tumblr.com/theme/39018)

Click the "Install" button and select the blog you would like the theme to be installed on.

With the theme installed, converting your Tumblr blog to a webcomic can be achieved in just two simple steps:

1. In the theme options, you will need to turn on “Comic Pagination”.
2. Scroll down and click on “Advance options”, set “Posts per page” to 1.

*Once you have published your first post you should copy and paste the post permalink into the "First Post URL" field. This ensures the comic pagination works correctly.*

Optional:
- To make your post image link to the next page, turn on "Clickable images".
- To include a random page link, turn on "Random button".

You can find a full breakdown of all the options here: [https://github.com/geoneo1/SimpleWebcomicTheme/blob/master/SWC_THEME_OPTIONS.md] (https://github.com/geoneo1/SimpleWebcomicTheme/blob/master/SWC_THEME_OPTIONS.md)

<a name="ComicPagination">
### The comic pagination is not showing up
In order for the comic pagination to appear, you need to have more than one post. I suggest having three posts to test all four of the buttons. 

<a name="ComicPaginationSmall">
### The comic pagination buttons are appearing very small
You can increase the height of your comic pagination images by changing the number in the "Comic pagination image height" field. The default is 24(px). Once you increase that, they will display larger.

<a name="PageLink">
### Is there a way to add a link to my first comic page in the navigation bar? 
1. Go to the Edit theme area
2. Scroll all the way down to the bottom and click “Add a Page” button
3. Click on the “Standard Layout” dropdown and select “Redirect”
4. Click the “Show a link to this page” toggle button
5. Once that is on you will be able to name your link
6. In the first field you can choose a custom URL
8. Then in the “Redirect to” field paste the URL of your first comic page

<a name="AskLink">
### How do I show the “Ask” link?
The theme does have an ask feature, but the setting is hidden away in the general tumblr options. 

In your tumblr dashboard, in the top right you should see a user icon (next to the lightning bolt). Click on that and select “Edit appearance”. The 4th option down is “Ask”, Make sure “Let people ask questions” is activated. Once it is, the link should appear in the theme automatically.

---

###### Trouble Shooting

<a name="FirstButtonURL">
### The “First” button is going to the wrong page
You must add the *post URL* in the “First comic page URL” field, not the *page URL*.

Go to your first comic page and click on either the date or the the link icon. Then just copy the URL and paste it into the "First comic page URL" field. Then save.

<a name="FirstButtonDisappeared">
### My “First” button has disappeared
Shortly after launching the theme a user bought to my attention that the first blog post may not necessarily be the first comic page. So I implemented a theme change to factor that in. 

Originally, as long as you had more than one post, the “First” button would show up, regardless if you filled in “First post URL” or not. Now, you *have to include the post URL* of your first comic page in the theme field “First comic page URL” in order for the “First” button to appear. 

Furthermore, as I changed the field name from “First post URL” to “First comic page URL” Tumblr treats it as a completely new field. The data you may have already entered is cleared requiring you to put it in again. 

<a name="ShowShareButtons">
### I can't see my share buttons
Make sure that the “Post metadata" option is turned on. The Post metadata includes the *author*, *time stamp*, *tags*, *notes*, *comment count*, *content source*, as well as all the *share options*. The theme has options to individually hide these features.

<a name="ShowBannerImage">
### My banner image is not showing
1. Go to the Edit theme area 
2. Make sure “Show header image" is on

If you are using one large image:

- Make sure “Repeat header” image is off
- You can adjust "Header height” option to better suit your image

*Note: If you are using “Big header” It will override the Header height option.*

<a name="GoogleLink">
### My Google+ link is not going to the correct URL
For “Google Plus Username” to work you will require a *Google+ Custom URL*. Please take a look at [Getting Started with Google+ Custom URLs] (http://goo.gl/9oRRRH).

<a name="SocialLinksColours">
### My “Show social links” is on, but I can't see the logo (picture) of each social links

The background of the social links are determined your “Accent color”, the icons are determined by your “Aside text” colour, if these two are the same colour, you will not be able to see the icons. However, you can change the colour of the background. 

Go to the Edit theme area, scroll to the bottom and click “Advanced options”, then copy and paste the following into the “Add custom CSS” field:
```
.social-links ul li a span.ico { background-color: #222; }
```
If you prefer to keep the background as is and change the icon colour instead, paste this:
```
.social-links ul li a { color: #fff; }
```

<a name="GoogleAnalyticsStatus">
### Why does my Google Analytics status read “Tracking code not verified”?
After adding the your Google Analytics tracking code in your theme options, it may take 24 hours for data to appear in your reports.

---

###### Design

<a name="TransparentHeader">
### Is there a way for the header and aside to have a transparent background?
Go to the Edit theme area, scroll to the bottom and click “Advanced options”, then copy and paste the following into the “Add custom CSS” field:
```
header#masthead, .alternative aside, .alternative footer.sub-basement { background-color: transparent; }
```
This removes the shadow from the Header (should you want to):
```
header#masthead > div { box-shadow: none; }
```

<a name="CenterNavigation">
### How can I center the navigation links?
Go to the Edit theme area, scroll to the bottom and click “Advanced options”, then copy and paste the following into the “Add custom CSS” field:
```
nav#access .wrapper { text-align: center; }
```

<a name="NavigationShadow">
### How do I get rid of the shadow under the navigation?
Go to the Edit theme area, scroll to the bottom and click “Advanced options”, then copy and paste the following into the “Add custom CSS” field:
```
nav#access { box-shadow: none !important; }
```

<a name="ComicPaginationSpace">
### How do I reduce the space above and below the comic pagination?
Go to the Edit theme area, scroll to the bottom and click “Advanced options”, then copy and paste the following into the “Add custom CSS” field:
```
.comic-pagination, .pagination { padding: 2em 0 0; }
footer.metadata { margin-top: 2em; }
```
In this case 2em equals 32px. I am using ems, you can use pxs if you are more comfortable with the. 

<a name="ContentTopPadding">
### How do I reduce the top padding in the content area?
Go to the Edit theme area, scroll to the bottom and click “Advanced options”, then copy and paste the following into the “Add custom CSS” field:
```
article { padding-top: 2em; }
```
*The default is 4em (which is 64px), in the example I have halved it, but you can change it to whatever suits you. You don't need to stick to ems either, you can use px if you prefer.*

<a name="ContentWidth">
### How do I increase the content width?
Go to the Edit theme area, scroll to the bottom and click “Advanced options”, then copy and paste the following into the “Add custom CSS” field:
```
article > *, div#disqus_thread, section#notes,
.alternative article > *, .alternative div#disqus_thread, .alternative section#notes {
  width: 80%;
}

@media only screen and (max-width:480px){
  article > *, div#disqus_thread, section#notes,
  .alternative article > *, .alternative div#disqus_thread, .alternative section#notes {
    width:90%
  }
}
```

<a name="ChronologicalOrder">
### Is there a way to make post show in chronological order?
I did look into adding this feature when I was building the theme, but as far as I am aware, tumblr does not allow theme builders this feature.

There is a way you can do it using tags  http://staff.tumblr.com/post/34933619/new-feature-tag-filtering

I usually advise people to create “Read from the beginning” link in the main nav that links to the first comic page URL. 

<a name="Disqus">
### Is there a way to add Disqus on the homepage?
Disqus comments only appear on the individual posts because they require a unique URL. If they were to appear on the homepage, when you add a new post, any previous comments will still be visible. Which may result in unrelated comments. 

If you still want it to appear on the homepage, there is a way but it would mean the comments will show on all pages, including any custom pages. 

If you still would like to add comments to pages: 

1. Go to the Edit theme area
2. Click on “Edit HTML”
3. Press CTRL+F, a search box should appear
4. Search for `<!-- Disqus -->`
5. You will see that 2 lines above it has `{block:PermalinkPagination}` - that line of code limits it to just individual post pages. You must remove that line
6. You must also remove its closing counterpart `{/block:PermalinkPagination}` which you will find just at the bottom of that section of code, just above `{block:IfPostNotes}` 
7. Save and exit

<a name="PageImageWidth">
### How can I have the images width on my custom page the same as the wrapper width? 
The content area of a page is 60% width of the full wrapper. In order to change that go to the Edit theme area, scroll to the bottom and click “Advanced options”, then copy and paste the following into the “Add custom CSS” field:
```
article > .caption, .alternative article > caption { width: 100%; }

article > .caption > p,
article > .caption > h2 {
  margin: 0 auto 1em;
  width: 60%;
}
.alternative article > .caption > p, .alternative article > .caption > h2 {
  width: 70%;
}
article > .caption > h2 {
  margin: 1em auto;
}
article > .caption > figure,
  .alternative article > .caption > figure {
  margin: 0 0 1em;
  text-align: center;
}
@media only screen and (max-width:680px){ 
  article > .caption > p,
  article > .caption > h2  { width: 70%; }
}
@media only screen and (max-width:480px){ 
  article > .caption > p,
  article > .caption > h2,
  .alternative article > .caption > p,
  .alternative article > .caption > h2 { width: 90%; }
}
```
If you upload an image using the tumblr page editor, it will automatically resize it to 500px width. The only way around that is if you upload the image somewhere else first and then in the “HTML edit” mode paste the correct image URL. You will also need to wrap the image in a `<h1>` tag. If you do not do this, then tumblr will automatically wrap it in a `<p>` which we don’t want.  

<a name="VisitedLinkColour">
### How do I change the clicked-link color? 
Go to the Edit theme area, scroll to the bottom and click “Advanced options”, then copy and paste the following into the “Add custom CSS” field:
```
a:visited { color: #ff0; }
```
<a name="PostAvatarSize">
### How can I expand the post author portrait in Simple Webcomic to make it bigger than 24x24?
1. Go to the Edit theme area
2. Click on “Edit HTML”
3. Press CTRL+F, a search box should appear
4. Search for `{PostAuthorPortraitURL-24}`
5. You have the option to change the size to 16, 24, 30, 40, 48, 64, 96, 128 
6. So if you wanted the size to be 40 you would swap 24 for 40 e.g. `{PostAuthorPortraitURL-40}`

<a name="WiderFooterSection">
### Is there a way to make the “About” section in the footer wider?
Go to the Edit theme area, scroll to the bottom and click “Advanced options”, then copy and paste the following into the “Add custom CSS” field:
```
aside section, .alternative aside section, .wrapper-slim aside section { width: 49%; }
```

2. Click on “Edit HTML”
3. Press CTRL+F, a search box should appear
4. Search for `<!-- Disqus -->`
5. You will see that 2 lines above it has `{block:PermalinkPagination}` - that line of code limits it to just individual post pages. You must remove that line
6. You must also remove its closing counterpart `{/block:PermalinkPagination}` which you will find just at the bottom of that section of code, just above `{block:IfPostNotes}` 
7. Save and exit

<a name="PageImageWidth">
### How can I have the images width on my custom page the same as the wrapper width? 
The content area of a page is 60% width of the full wrapper. In order to change that go to the Edit theme area, scroll to the bottom and click “Advanced options”, then copy and paste the following into the “Add custom CSS” field:
```
article > .caption, .alternative article > caption { width: 100%; }

article > .caption > p,
article > .caption > h2 {
  margin: 0 auto 1em;
  width: 60%;
}
.alternative article > .caption > p, .alternative article > .caption > h2 {
  width: 70%;
}
article > .caption > h2 {
  margin: 1em auto;
}
article > .caption > figure,
  .alternative article > .caption > figure {
  margin: 0 0 1em;
  text-align: center;
}
@media only screen and (max-width:680px){ 
  article > .caption > p,
  article > .caption > h2  { width: 70%; }
}
@media only screen and (max-width:480px){ 
  article > .caption > p,
  article > .caption > h2,
  .alternative article > .caption > p,
  .alternative article > .caption > h2 { width: 90%; }
}
```
If you upload an image using the tumblr page editor, it will automatically resize it to 500px width. The only way around that is if you upload the image somewhere else first and then in the “HTML edit” mode paste the correct image URL. You will also need to wrap the image in a `<h1>` tag. If you do not do this, then tumblr will automatically wrap it in a `<p>` which we don’t want.  

<a name="VisitedLinkColour">
### How do I change the clicked-link color? 
Go to the Edit theme area, scroll to the bottom and click “Advanced options”, then copy and paste the following into the “Add custom CSS” field:
```
a:visited { color: #ff0; }
```
<a name="PostAvatarSize">
### How can I expand the post author portrait in Simple Webcomic to make it bigger than 24x24?
1. Go to the Edit theme area
2. Click on “Edit HTML”
3. Press CTRL+F, a search box should appear
4. Search for `{PostAuthorPortraitURL-24}`
5. You have the option to change the size to 16, 24, 30, 40, 48, 64, 96, 128 
6. So if you wanted the size to be 40 you would swap 24 for 40 e.g. `{PostAuthorPortraitURL-40}`

<a name="WiderFooterSection">
### Is there a way to make the “About” section in the footer wider?
Go to the Edit theme area, scroll to the bottom and click “Advanced options”, then copy and paste the following into the “Add custom CSS” field:
```
aside section, .alternative aside section, .wrapper-slim aside section { width: 49%; }
```
