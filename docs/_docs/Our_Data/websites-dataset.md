---
title: NGO Websites Dataset
category: Our Data
menu_order: 1
order: 1
---

> Over 9k entities! (~15k NGOs in primary sample) <img src ="https://raw.githubusercontent.com/Teplitsa/CSRLab/main/docs/images/fire.png" width="30" height="30" alt="fire">

This dataset the most data was obtained from ["OpenNGO"](https://openngo.ru/) and enriched with SEO metrics collected by our lab. Other resources: SPARK-Interfax registrar, [tochno.st](https://tochno.st) by “Help Needed” Foundation, and Teplitsa beneficiaries data.

### Hypothesis:

* Russian NGOs do not use their digital communicative capacity to the fullest, even when it comes to the basic level SEOs <img src ="https://raw.githubusercontent.com/Teplitsa/CSRLab/main/docs/images/check.png" width="30" height="30" alt="check">

### Results:

* Younger organizations more often have social network 
pages
* Elder organizations’ websites are less optimized
* Charity foundations far more often have numerous social network pages
* Charity foundations and autonomous nonprofits have websites more optimized for search engines and with easier interfaces than other organization forms

You can download .csv dataset with seo metrics [here](https://github.com/Teplitsa/CSRLab/blob/main/data/2022_lab_index_report.csv). And the other part of dataset with parameters from OpenNGO [here](https://raw.githubusercontent.com/Teplitsa/CSRLab/main/data/2022_lab_selected_ngos_data.csv). The datasets can be joined by `ogrn` field. Online searchable database will be available in a few months.

### Dataset Structure:

```
{'ogrn': ,  # organisation registration number
 'website': ,  # NGO website url
 'bin_robots': ,  # does the website have a robots file (seo)? 
 'bin_sitemap': ,  # does the website have a sitemap (seo)?
 'bin_fb': ,  # does NGO have a facebook page?
 'bin_vk': ,  # does NGO have a Vkontakte page?
 'bin_ig': ,  # does NGO have an Instagram page?
 'bin_ok': ,  # does NGO have an Odnoklassniki page?
 'bin_youtube': ,  # does NGO have a Youtube page?
 'bin_tiktok': ,  # does NGO have a TikTok page?
 'bin_donation': , #
 'wcag_score': ,  #
 'mean_page_speed': ,  #
 'bin_title': ,  #
 'bin_headings': ,  #
 'bin_mob_friendly': ,  #
 'bin_ssl': ,  #
 'bin_socnet': ,  #
 'websiteCreationDate': ,  # website creation date
 'regionName': 'Волгоградская область', # in which region of Russia NGO is registered
 'minjustForm': 'Автономная некоммерческая организация',  # a legal form of organisation
 'regDate': ,  # Registration date. Exists only for organisations registered before 2002
 'shortName': 'АНО ФКВС "ВОЛГА"',  # short name of organisation with abbrebiations
 'mainOkved': ,  # ОКВЭД="All-Russian Classificator of Economic Activity Types"
 'opfCombined': ,  # Organisation type according to ЕГРЮЛ data="Official Registrar of Legal Entities"
 'okvedCombined': ,  #  ОКВЭД="All-Russian Classificator of Economic Activity Types" if more than one and have detailed addOkved
 'vedSimple': ,  # manually defined more generic organisation type based on ЕГРЮЛ and ОКВЭД data
}
```

