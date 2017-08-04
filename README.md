# Web-Crawling-in-Python
This code is to use Python 3.5 to use the web spider to iteratively find and fetching web links starting from target URL.<br><br>

In command prompt, run the following command: > python webCrawl.py <link> <br>
assume the target url is  http://www.w3schools.com <br>

```
> python webCrawl.py www.w3schols.com 
```
By default, it will fetch 1000 different urls directly or indirectly linked to target url and output links on links.txt <br>
You can check the file "links.txt" I uploaed.  <br>

It can be customized fetch by using following optional tag: <br><br>

fetch number of urls <br>
-n number
```
> python webCrawl.py www.w3schols.com  -n 300 
```
Assign url prefix <br>
-p prefix 
```
> python webCrawl.py www.w3schols.com  -p http://www.w3schools.com/js/ 
```
Assign url key word.<br>
-k keyword  
```
> python webCrawl.py www.w3schols.com  -k javascript
```
Assign url extension <br>
-e extension
```
python webCrawl.py www.w3schols.com  -e .asp 
```
Assign output file<br>
-f output_filename <br>
```
> python webCrawl.py www.w3schols.com  -f inks_w3school.com 
```

For exmpample, I'd like to crawl www.w3schools.com and I hope the key word is  and n is 500. <br>

The command will be <br>
```
> python webCrawl.py www.w3schools.com  -n 500  -k css  -f links_w3schools_css_500.txt
```
So this program will use spider to crawl 500 different url and output the urls with key word "css".  <br>
Please check the file links_css_500.txt <br><br>



By the way, before you run it, please make sure you install Python 2.7 or 3.5 and install BeautifulSoup <br>
Here is the steps for install Python 3.5 and Beautiful.<br>

1. Install Python 3.5 from http://conda.pydata.org/miniconda.html <br>
2. install anaconda and update conda, anaconda (please see the attached slide) <br>
In command prompt, run the following command: <br>
```
> conda install anaconda 
```
3. . Install bs4 library, after install Python 3.5 from conda <br>
In command prompt, run the following command <br>
```
> conda install -c anaconda beautifulsoup4=4.5.1 
```
