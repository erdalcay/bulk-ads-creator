## Google Sheets Based Ads Script for Bulk Ad Creation 

Originally published at: **(TR)** [Blog Post](https://zeo.org/tr/blog/google-ads-script-toplu-reklam-olusturucu/)

Original repo: [https://github.com/zeoagency/bulk-ads-create](https://github.com/zeoagency/bulk-ads-create)

---- 

This script creates new expanded text ads under given ad groups using a Google Sheets file.
 
Here is the spreadsheet template you need to use (either by making a copy or creating it from scratch with exact column order):

[https://docs.google.com/spreadsheets/d/1jExrloljobQrR7uw0qrmDoMBt21IyBVafIzAZdlEnsM](https://docs.google.com/spreadsheets/d/1jExrloljobQrR7uw0qrmDoMBt21IyBVafIzAZdlEnsM)

### Usage

Start with inserting the spreadsheet URL and the name of the page that contains the ads.

```javascript
...

var spreadsheetURL = 'SPREADSHEET_URL';

var sheetName = 'Sheet1';

...
```

Next, tell the script whether you are running it under an MCC account or a single Google Ads account.
Change the below value to `true` if you are in your agency/business MCC or leave it as `false` if you are running the script in your Google Ads account.

```javascript
...

var isMcc = false;

...
```

Finally, enter the Google Ads account ID below if you are in an MCC account.

```javascript
...

var gAdsCustomerId = 'XXX-YYY-ZZZZ';

...
```

That is all, you are done!

Save and run it.
