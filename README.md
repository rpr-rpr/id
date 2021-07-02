# Creating a "man in the middle" page to track experimental interventions via Google Analytics

## Step 1 - Create a new page
* Click on the "Add file" button and select the "Create new file" option
* Name your file using a meaningful name by typing it in the "Name" textbox in the upper left corner of the screen, above the code textarea.

## Step 2 - Copy the code in the new page
* Copy/Paste the following code in the code textarea

```html
<html>
<head>
<!-- Global site tag (gtag.js) - Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=UA-180595550-1"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'UA-180595550-1');
</script>
<meta http-equiv="refresh" content="1; URL='Add link here'" />
</head>
</html>
```

## Step 3 - Change the link of the HTML redirect
* Go to line X and replace the "Add link here" by the url of the page you want to redirect to
* Scroll to the bottom of the page and click the "Commit new file" button

## Step 4 - Repeat Steps 1 to 3 for each interventions and the control

## Step 5 - Test the pages

The Url of the new pages will be following this format:

* https://rpr-rpr.github.io/id/[Name].html
