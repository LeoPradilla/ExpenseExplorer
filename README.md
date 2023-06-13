# Peronal Budget

<p align="justify">Since coming to Canada (and before that), I have been keeping a tight budget and tracking all my expenses. In the past, I tried different apps and methods, but the one that worked for me was the old, good, and reliable spreadsheets. I've been using Google Sheets as my expense tracker (Google even gives you a template you can use), and for the last 8 months, I have logged every single transaction meticulously. I believe I have gathered enough data to mine valuable insights from my spending habits.</p>

## Collecting the Data

<p align="justify">Using the Google API to connect to Google services provides secure access to your information on Google Sheets. You need to set up the environment, enable the API, create credentials, install libraries, and a couple of other things. Fortunately, Google offers comprehensive documentation to achieve this using Python (or several other languages). The complete guide can be found <a href="https://developers.google.com/sheets/api/quickstart/python#configure_the_sample">here</a>.</p>

<p align="justify">To gather information from the spreadsheets, you will need the spreadsheet ID and the range of cells where the information is stored within the spreadsheet. In my case, I prefer to organize my budget on a monthly basis, so I have a separate sheet for each month of the year. Fortunately, I am using a template where the range of cells remains the same across all the spreadsheets. I created a simple CSV file with two columns: one for the name of the month and another for the corresponding spreadsheet ID.</p>

<p align="center">
  <img src="images/sheets_csv.png" style="height:182px; width:532px"/>   
</p>
<p align="center">
    <em>Spreadsheet IDs</em>
</p>

Note: One easy method to know the ID of your spreadsheet is to look for it in the URL of your spreadsheet. For example, for this spreadsheet: `https://docs.google.com/spreadsheets/d/1XVqFHuHWjps-aq2VremvHPVY2G9MpD24U9s1mV3H_qU/edit#gid=0` the ID is `1XVqFHuHWjps-aq2VremvHPVY2G9MpD24U9s1mV3H_qU`
