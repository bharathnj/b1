
# Installation:
Requires Python 2.7. (Need Collections.Counter)
```
sudo pip install pyteaser
```

These dependency packages will be automatically installed:
```
Pillow
lxml
cssselect
jieba
beautifulsoup
```
Note: if you're installing on Windows, you have to install one of the dependency package lxml manually using:

```
easy_install lxml==2.3.3
```


# Usage:
## sample command:
```Python
>>> from pyteaser import SummarizeUrl
>>> url = 'http://www.huffingtonpost.com/2013/11/22/twitter-forward-secrecy_n_4326599.html'
>>> summaries = SummarizeUrl(url)
>>> print summaries

```

## output
```
["Twitter\'s move is the latest response from U.S. Internet firms following disclosures by former spy agency contractor Edward Snowden about widespread, classified U.S. government surveillance programs.", "\\"Since then, it has become clearer and clearer how important that step was to protecting our users\' privacy.\\"", "The online messaging service, which began scrambling communications in 2011 using traditional HTTPS encryption, said on Friday it has added an advanced layer of protection for HTTPS known as \\"forward secrecy.\\"", "\\"A year and a half ago, Twitter was first served completely over HTTPS,\\" the company said in a blog posting.", " \\"I\'m glad this is the direction the industry is taking.\\" \\n\\n(Reporting by Jim Finkle; editing by Andrew Hay)"]

```

you can use Summarize(title, text) directly if you already have the text and the title. Otherwise you must install Python Goose to extract text from url.
