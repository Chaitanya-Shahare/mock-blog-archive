---
title: How to add social media preview to website
layout: default
date: 24/10/2022
---

You might have come across some websites that when shared on social media platforms like Twitter & WhatsApp shows a preview card of the website which typically includes an image and a short description of the page. This is accomplished with the use of OpenGraph protocol. This is used to add meta data to your websites.

## How to add social media preview

This is done by adding OpenGraph meta tags to the `<head>` tag of the HTML file. For example:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
      <title>Page Title</title>
      <meta name="description" content="This is the description of the site.">
      <meta property="og:url" content="url">
      <meta property="og:title" content="Page Title">
      <meta property="og:type" content="website">
      <meta property="og:image" content="image url">
      <meta property="og:url" content="url">
      <meta property="og:description" content="This is the description of the site.">
      
  </head>
  <body>
  </body>
</html>
```

## Some basic OpenGraph properties

### **og:title**

```html
<meta property="og:title" content="Page Title">
```
This is used to add title, usually the same as the title of the page in `<title>` tag.

### **og:type**

```html
<meta property="og:type" content="website">
```
This is used to add information about what type of page the URL is for. It can be website, article or video.

### **og:image**

```html
<meta property="og:image" content="img_address">
```
This is used to add image to the preview by adding the image URL.

### **og:url**

```html
<meta property="og:url" content="url">
```
This property contains the URL of the current page.

### Other

There are various other open graph properties like og:description, og:domain, etc. Also there are some special platform specific properties like in the case of twitter.

### **twitter:card**

```html 
<meta name="twitter:card" content="summary_large_image">
```
This gives a large image with summary when the website url is shared on twitter.

## Easier way

You can use websites like https://www.opengraph.xyz to generate open graph meta tags for your website and customise it.

## How to check 

You can check if your site's opengrah tags are working on sites like [twitter card validator](https://cards-dev.twitter.com/validator) & [Facebook sharing debugger](https://developers.facebook.com/tools/debug/)


For detailed documentation refer to https://ogp.me .

[Next post](./posts/newpost.md)




