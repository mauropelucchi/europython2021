# Data Ingestion and Big Data @ EUROPYTHON 2021
## Build a dataset from zero to solid

![](https://raw.githubusercontent.com/mauropelucchi/europython2021/main/img/logo.png)

Web scraping, crawling and API are the first step to retrieve information to use for analysis
and to start a new business.
In this tutorial I'll show you how to use python to set up scraping and crawling processes,
how to simulate users navigation and browser behavior with a ghost browser and how to hook up and use data APIs.
I will also try to explain the technical and ethical aspects that we have to consider when we approach these kinds of challenges.

## About

This repo contains slides and code for Mauro Pelucchi's "Data Ingestion and Big Data" @ EuroPython 2021.

- [Access slides](https://github.com/mauropelucchi/europython2021/blob/main/slide/EUROPYTHON2021_BigData_Data_Ingestion.pdf)
- [Access notebook (colab)](https://github.com/mauropelucchi/europython2021/blob/main/notebook/EUROPYTHON_2021_Web_Scraping_with_Selenium.ipynb)

## Running the notebook

I **highly** recommend using the Colab, but in case you want to do it on your local notebook, follow the steps below:

1. Download ChromeDriver [https://chromedriver.chromium.org/downloads](https://chromedriver.chromium.org/downloads)
2. Import these libs

```
import sys
import logging
from selenium.webdriver.remote.remote_connection import LOGGER
LOGGER.setLevel(logging.WARNING)
from selenium import webdriver
from tqdm import tqdm_notebook as tqdm
import pandas
import json
import pprint
```
3. Create your ChromeDriver
```
wd = webdriver.Chrome('<path where you stored chromedriver>/chromedriver',chrome_options=chrome_options)
```

# MIT License

Copyright (c) 2021 Mauro Pelucchi

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.