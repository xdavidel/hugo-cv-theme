# DD CV Theme
Theme to build a customizeable printable HTML/CSS CV.

# Features
 - Online CV with minor responsiveness
 - Printable as A4 PDF
 - HTML5 + CSS3
 - Customizeable colors

## Print your PDF CV
When printing the page in the browser, you'll get a formatted A4 page that can be used as your PDF resume.
If your page holds more than 1 A4 page, the content will be divided into the given amount of pages.

For better formatting, you can set the number of pages in the `config.toml` file.

```toml
pages = 2
```

If badges and other elements with background don't render correctly, remember to toggle the "Background Graphics" option in the print dialog.

# Usage
## Install Hugo (extended)
To use `hugo-cv-theme` theme you need to install __Hugo Extended__ by following https://gohugo.io/getting-started/installing/.

## Create your personal website
```
hugo new site <your website's name>
cd <your website's name>
git init
git submodule add https://github.com/xdavidel/hugo-cv-theme.git themes/dd-cv
```

## Start Hugo in development mode
```
hugo server -D
```
Your site is now available at http://localhost:1313/.

## Customization
Your professional data should be added in the `data/content.yaml` file. 
You can change the theme colors and number of pages in the `config.toml` file.

For more advanced customization, in your site root directory create `assets/scss/_custom.scss` file where you can
overwrite theme SCSS as per your liking.

## Building
To generate static files of your website, execute the following:
```
hugo --minify
```
within the root of your project.

# Thanks
This theme is being reforge from another project [almeida-cv](https://github.com/ineesalmeida/almeida-cv)
Please view the original creator hard work. 