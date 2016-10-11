# Web-Crawling-in-Python
This code is to use Python 3.5 to use the web spider to iteratively find and fetching web links starting from target URL.<br><br>

In command prompt, run the following command: > python webCrawl.py <link> <br>
assume the target url is  http://www.w3schools.com <br>

&gt; python webCrawl.py www.w3schols.com <br>
or <br>
&gt; python webCrawl.py http://www.w3schols.com <br>
By default, it will fetch 1000 different urls directly or indirectly linked to target url and output links on links.txt <br>
You can check the file "links_w3schools.com" I uploaed.  <br>

It can be customized fetch by using following optional commands: <br>
-n [number]:  fetch number of urls. e.g. &gt;python webCrawl.py www.w3schols.com  -n 300  <br> 
-p [string]: assign url prefix. e.g. &gt;python webCrawl.py www.w3schols.com  -p http://www.w3schools.com/js/  <br>
-k [string]: assign url key word. e.g &gt;python webCrawl.py www.w3schols.com  -k array <br>
-e [sring]: assign url extension. e.g.&gt; python webCrawl.py www.w3schols.com  -e .asp <br>
-f [string]: assign output file. e.g &gt; python webCrawl.py www.w3schols.com  -f inks_w3school.com <br> <br>

For exmpample, I'd like to crawl www.w3schools.com and I hope the key word is bootstrap and n is 500. <br>

The command will be<br>
&gt; python webCrawl.py www.w3schools.com  -n 500  -k bootstrap  -f links_bootstrap_n=500.txt <br>

So this program will use spider to crawl 500 different url and output the urls with key word "bootstrap".  <br>
Please check the file links_bootstrap_n=500.txt <br>

By the way, before you run it, please make sure you install Python 2.7 or 3.5 and install BeautifulSoup <br>
Here is the steps for install Python 3.5 and Beautiful.<br>

1. Install Python 3.5 from http://conda.pydata.org/miniconda.html <br>
2. install anaconda and update conda, anaconda (please see the attached slide) <br>
In command prompt, run the following command: <br>
&gt; conda install anaconda <br>
3. . Install bs4 library, after install Python 3.5 from conda <br>
In command prompt, run the following command <br>
&gt; conda install -c anaconda beautifulsoup4=4.5.1 <br> 
