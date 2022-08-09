# Datasets column description

`2021_sep_egrul_initial_dump (ngos websites)`
- **Наименование**: organization name (if registered in company register)
- **Регистрационный номер**: OGRN registration number in company register)
- **Наименование на английском**: organization name in English
- **Краткое наименование**: organization short name
- **Наименование полное**: organization full name
- **Адрес (место нахождения)**: organization address
- **Сайт в сети Интернет**: organization website
- **Дата регистрации**: organization registration date
- **Код налогоплательщика**: INN registration tax ID
- **Регион регистрации**: organization registration region (in Russia)
- **Вид деятельности/отрасль**: OKVED (Russian Classification of Economic Activities)
- **Организационно-правовая форма**: OKOPF (Russian National Classifier of Forms of Incorporation)

`2022_lab_index_report.csv`
- **ogrn**: OGRN registration number in company register)
- **website**: link to website
- **bin_robots**: robots.txt found on website (1/0)
- **bin_sitemap**: sitemap.xml found on website (1/0)
- **bin_fb**: Facebook page link found on website (1/0)
- **bin_vk**: Vkontakte page link found on website (1/0)
- **bin_ig**: Instagram page link found on website (1/0)
- **bin_ok**: Odnoklassniki page link found on website (1/0)
- **bin_youtube**: Youtube page link found on website (1/0)
- **bin_tiktok**: Tiktok page link found on website (1/0)
- **bin_donation**: donations page found on website (1/0)
- **wcag_score**: WCAG test complex score from Lighthouse
- **mean_page_speed**: page speed test complex score from Lighthouse
- **bin_title**: <title> tag used on website pages (1/0)
- **bin_headings**: <h1-h6> tags used on website pages (1/0)
- **bin_mob_friendly**: mobile friendliness test from Google devs (1/0)
- **bin_ssl**: ssl certificates on website (1/0)
- **bin_socnet**: any social network page link found on website (1/0)
  
`2021_dec_vk_parsed.csv`
- **vk**: Vkontakte page link found on website
- **count_members**: total members count
- **count_posts_all**: total posts count
- **count_posts_per_month**: mean posts per month
- **likes_overall_all**: total likes count
- **likes_mean_all**: mean likes per post
- **comments_overall_all**: total comments count
- **comments_mean_all**: mean comments per post
- **reposts_overall_all**: total reposts count
- **reposts_mean_all**: mean reposts per post
- **views_overall_all**: total views count
- **views_mean_all**: mean views per post
- **ads_overall_all**: total ads launched

`ngos_cities_of_hostings.csv`
- **website**: link to website
- **websiteCreationDate**: website creation date (whois data)
- **website_country**: 
- **website_hostname**: website hosting provider
- **website_isp**: Internet Service Provider (ISP) 
- **website_city**: 
- **website_latitude**: 
- **website_longitude**: 
 
`2021_dec_social_networks_check.csv`
- **url**: link to website
- **fb**: Facebook page found on the website
- **vk**: VK page found on the website
- **ig**: Instagram page found on the website
- **ok**: Odnoklassniki page found on the website
- **youtube**: Youtube page found on the website
- **tiktok**: Tiktok page found on the website

`2021_dec_wcag_test.csv`
- **id**: WCAG test feature id from Lighthouse
- **title**: WCAG test feature desc from Lighthouse
- **score**: WCAG test score from Lighthouse
- **website**: link to website
  
`2021_lab_websites_cms.csv`
- **ogrn**: OGRN registration number in company register)
- **website**: link to website
- **CMS**: CMS used
