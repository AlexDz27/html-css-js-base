# Running the app
Needs web server, e.g. `php -S localhost:8085 -t .`

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