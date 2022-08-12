# [Civil Society Research Lab](http://lab.te-st.ru/)

### Aim

The CSRLab is a data-driven research project for the Russian civil society online communication practices.

> ** Mission:** evaluating of communicative capacity of the Russian-language third sector and establishing best communicative practices. The communicative capacity indicates the organization’s ability to undertake work aimed at conveying the most important information to beneficiaries, donors, and society at large (especially if the organization engages in advocacy work).

The CSRLab focuses on the online communications of the third-sector via their websites and social media. We investigate both officially established organizations (registered by Russian authorities as a non-commercial organization) and non-registered communities of activists and their organistaions. Examples of the later communities is anti-war and humanitarian movements that multiplied across Russia and abroad after Russia invaded Ukraine in Februrary 2022.

### Data

> ** non-reactive data** collected by means of web scrapping and through APIs. The use of non-reactive data is a principle demand for us, an effort to overcome the limitations of previous studies that used biased samples or self-survey data. By collecting and analyzing data in house, we try to avoid subjective assessments made by NGO representatives.

By August 2022 our sample contains 13k+ :fire: organizations and communities (both legally registered in Russia and not-registered legally anywhere).

This repository contains data collected by the CSRLab, scripts for data mining and transformation, and infographics. Narrative reports (in Russian) on data gathering and processing are published on the Lab website - [lab.te-st.ru](http://lab.te-st.ru/u). English short version of reports are present on [github pages](https://teplitsa.github.io/CSRLab/).


| folder  | content |
| ------------- | ------------- |
| `data` | data collected on websites and domain names, Russian including company register data, WCAG and speedtests, SEO tests, whois check  |
| `notebooks`  | research journaling  |
| `source-code`  | scripts for data mining and processing  |
| `plots`  | infographics  |
| `Skillfactory x Teplitsa Lab`  | datasets collected for Skillfactory hackathon |

### Methods used
- data scraping, processing and cleansing
- descriptive statistics
- inferential statistics
- social network analysis
- data visualization

### Technologies
- python
- pandas, jupyter
- plotly, seaborn, gephi
- MongoDB
- OpenRefine

---------

# [Лаборатория исследований гражданского общества](http://lab.te-st.ru/)  

Лаборатория создана в рамках «Теплицы социальных технологий» в 2021 году для изучения практик онлайн-коммуникации гражданского общества, в частности, зарегистрированных в России некоммерческих организаций. Мы исследуем онлайн-коммуникации некоммерческих организаций. Чтобы оценить, как организации общаются в интернете со своей аудиторией, мы разработали собственную методику. Мы собираем нереактивные данные о коммуникации (data mining), что позволяет нам избежать субъективных оценок представителей самих НКО о том, как устроены их коммуникации и какой эффект они могут иметь.

В данном репозитории хранятся данные, собранные Лабораторией, скрипты для их получения и преобразования, инфографика. Повествовательные отчеты о работе лаборатории с данными опубликованы на официальном сайте Лаборатории [lab.te-st.ru](http://lab.te-st.ru/). 

В августе 2022 в нашей выборке:

- 13k+ вебсайтов
- 3k+ страниц VK
- 3k+ страниц FB
- 3k+ страниц Instagram
- 7k+ каналов Telegram

| папка  | содержимое |
| ------------- | ------------- |
| `data` | собранные данные о вебсайтах, включая данные ЕГРЮЛ, тестов скорости загрузки и WCAG, speedtests, SEO tests, whois  |
| `notebooks`  | журналы исследований  |
| `source-code`  | скрипты для скачивания и преобразования данных |
| `plots`  | графики  |
| `Skillfactory x Teplitsa Lab`  | данные собранные во время хакатона Skillfactory |

### Методы
- скрейпинг, предобработка и очстка данных
- описательная статистика
- статистический вывод
- анализ социальных сетей
- визуализация данных

### Инструменты
- python
- pandas, jupyter
- plotly, seaborn, gephi
- MongoDB
- OpenRefine
