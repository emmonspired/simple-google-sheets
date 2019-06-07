# simple-google-sheets
A utility for handling authentication and retrieval of google sheets data.

```
const {SimpleGoogleSheets} = require('simple-google-sheets');

const sheets = new SimpleGoogleSheets({
    SCOPES: ['https://www.googleapis.com/auth/spreadsheets.readonly'],
    CREDENTIALS_PATH: './credentials/google-sheets-credentials.json',
    TOKEN_PATH: './credentials/google-sheets-token.json'
});

let rows = sheets.getRowsWithCredentials({spreadsheetId:'somesheet',range:'Site Defaults!A1:J'});
```
