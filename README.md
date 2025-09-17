# Running the app
## Standard way
Needs web server, e.g. `php -S localhost:8085 -t .`
## File way
If you want to work with the project just like with regular files opened via browser,
simply remove first slash from the assets in <head>

# Changelogs
## 2025-06-30 20:22
Added assets/, fonts, and './' starting path. 
The path now works both for local and web-server setups (previously was only working for local)

## 2025-07-01 18:11
Added img folder, some console.log in main.js

## 2025-07-07 20:17
Remove empty lines
Add input
Add STYLES section

## 2025-07-13 16:50
Found out that if using ./ paths, there will be problems with urls like localhost/qwe/asd -- the assets will be downloaded from /qwe/assets, which is wrong -> we need to use just '/' instead of './'.
The downside of this is that locally for development i will need to set up webserver rather than simply relying on the path of index.html itself.

## 2025-07-25 20:49
- html fz for rems to work properly
- btn display-block to prevent situations when i apply .btn on label, and wonder wtf happened with width (bc label is inline, not inline-block)

## 2025-08-06 12:51
Reasoning for putting js into assets: it's just more convenient project structure wise. And historically wise.
Yes, it may require some business-logic (like fetches), but it is still
an *asset* to the site.

*2025-08-06 13:20*: font-size should be in html cuz if in body rems won't work.
Added heap.css for placing under-development components into heap, and then to possibly porting them into separate css files (like btn.css)

## 2025-08-22 13:38
Add img {width: 100%}. TODO: make commit. It's better to have it because it's more expected behavior from an image, rather than default browser behavior when it overflows the box of the parent element.

## 2025-09-17 21:59
Add color: inherit to .btn