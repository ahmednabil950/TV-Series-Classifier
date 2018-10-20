# TV-Series-Classifier
Arabic TV Series Detection [App](http://series-detection.herokuapp.com/) trained on TV web pages.
<br>
<br>
<br>
<br>
<div align="middle">
<figure>
<img src='https://github.com/ahmednabil950/TV-Series-Classifier/blob/master/img/demo.PNG' alt='Web Demo' align="middle">
<br>
<figcaption>Fig.1 - WEB DEMO</figcaption>
</figure>
</div>

# Abstract
This repository contains experiment about a project i was doing about TV Series Classification from any given web page.
<br>
The target web page the model can recognize is **[Ra7eem TV Series](https://www.facebook.com/rahem.series/)** related web pages
<br>
<br>
<br>

# Features Engineering
In my experiment through building models before in topic modeling problems i prefer TfIdf features vectorization to CountVectorizer (normal BOW) due to it weights the important features which is relevant to the context of the web pages that is used to build the model. So better performance is obtained.
<br>
There is many features that is not very important like shown in the next captions and it can be treated like stopwords so better features realization is obtained.
<br>
<br>
<br>


# Classifier
<div align="middle">
<figure>
<img src='https://github.com/ahmednabil950/TV-Series-Classifier/blob/master/img/train.png' alt='Web Demo' align="middle">
<br>
<figcaption>Fig.2 - Training performance</figcaption>
</figure>
</div>


<div align="middle">
<figure>
<img src='https://github.com/ahmednabil950/TV-Series-Classifier/blob/master/img/test.png' alt='Web Demo' align="middle">
<br>
<figcaption>Fig.3 - test performance</figcaption>
</figure>
</div>


<br>
<br>
<br>

```
Examples you can test with and were not in the training set:
https://mzarita.tv/watch.php?vid=dfa569e72
https://moviz4u.tv/
https://www.elcinema.com/work/2048748
http://www.masrawy.com/ramadan/Tag/797735/%D8%B1%D8%AD%D9%8A%D9%85
http://www.masrawy.com/ramadan/drama-news/details/2018/6/16/1376870/%D8%A8%D8%A7%D9%84%D9%81%D9%8A%D8%AF%D9%8A%D9%88-%D9%83%D9%88%D8%A7%D9%84%D9%8A%D8%B3-%D9%82%D8%AA%D9%84-%D8%B1%D8%AD%D9%8A%D9%85-%D9%81%D9%8A-%D8%A7%D9%84%D8%AD%D9%84%D9%82%D8%A9-%D8%A7%D9%84%D8%A3%D8%AE%D9%8A%D8%B1%D8%A9-#keyword
```

<br>
<br>
<br>


# Data
### Data fetching
The data is obtained through Scrapper library from any web page. The used scrapper i preferred in my experiment is [BeautifulSoup4](https://www.crummy.com/software/BeautifulSoup/).
<br>

### Missing data
There is many approaches to handle the missing data, The good practise recommend not to ignore the missing rows in the dataset since it will affect the learned parameters through the optimization.
In my case the missing data was 1.12 % of the whole dataset so for sake of simplicity i dropped them.
Otherwise, other cases could be handled like filling random numbers that represents features in those missing entries.
<br>
<br>
<br>


# USAGE
* navigate to live [App](https://series-detection.herokuapp.com/) to test.
