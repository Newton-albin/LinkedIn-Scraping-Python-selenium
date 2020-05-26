# LinkedIn-Scraping-Python-selenium
Download the chrome driver using the below link:

https://chromedriver.chromium.org/

now we access the chrome browser using the code
```
driver=webdriver.Chrome()
driver.get("https://www.linkedin.com")
```
install selenium for web scraping
```
pip install selenium
```
In our project we are performing the  following actions:

1.SIGNIN the linkedin account.

2.Search for Python jobs and scrape the urls of 10 profiles.
```
driver.get('https://www.google.com')
search_box=driver.find_element_by_name('q')
search_box.send_keys(details.search_query)
```
3.Open every url in linkedin,and scrape the name and  contact. For this we are installing parsel module.
```
pip install parsel
```
4.Scrape the email id.

5.Store the profile urls, name, emailid in the excelsheet.For this we are using xlsxwriter module.
```
pip install XlsxWriter
```
6.Sending email to those scraped emailid with the attachment(resume) file.
```
import smtplib
from email.mime.text import MIMEText
from email.mime.multipart import MIMEMultipart
from email.mime.base import MIMEBase
from email import encoders
import os.path
```
7.Process completed.


