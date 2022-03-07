# How-to 

## Install Ghost
```
npm install -g ghost-cli
```


## Install Gscan 
```
npm install -g gscan
```

## Gscan theme
```
gscan /path/to/ghost/content/themes/casper
```

# Creating a new theme 
- Create a new folder for the theme under content/themes and create the theme layout.
- Create a package.json file and set metadata of the theme.
- Add three files named default.hbs, index.hbs and post.hbs and write some code to display the blog content.
- Restart the Ghost installation.
- Login as Ghost admin and activate the custom theme.


# Theme Templates 

* default.hbs - base template that contains the HTML markup (Outline) that exists on every page such as <html>
* index.hbs - It is used to display the list of posts. This template will be used if your theme does not have a tag.hbs, author.hbs or index.hbs page template.
* home.hbs - home.hbs act as the home page of a blog. It's an optional template
* post.hbs - template for a single post which extends default.hbs and uses the {{#post}} helper to output the post details.
* page.hbs - optional template for static pages. If this is not specified then post.hbs will be used.
* author.hbs - if not specified the index.hbs template is used
* private.hbs - optional template for the password form page on password-protected publications
* error.hbs - This theme template is used to display 404 or 500 errors that are not handled by error- or class-specific templates.
* tag.hbs - optional template for tag archive pages. If not specified the index.hbs template is used.
* amp.hbs - optional theme template for AMP (Accelerated Mobile Pages). If your theme doesn't provide an amp.hbs file, Ghost will use its default.
  
 
# GrapesJS
GrapesJS is a multi-purpose, Web Builder Framework, which means it allows you to easily create a drag & drop enabled builder of "things". By "things" we mean anything with HTML-like structure https://www.npmjs.com/package/grapesjs
  
```
npm i grapesjs-cli
npx grapesjs-cli serve
```
