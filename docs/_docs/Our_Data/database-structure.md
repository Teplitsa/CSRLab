---
title: Overall Database Structure
category: Our Data
menu_order: 1
order: 2
---

> The database will be publicaly available in several months with ability to send search queries. We hope that other researchers will be interested in investigating this data and contributing to it <img src ="https://raw.githubusercontent.com/Teplitsa/CSRLab/main/docs/images/hugging_face.png" width="30" height="30" alt="hugging_face">

We use MongoDB <img src ="https://raw.githubusercontent.com/Teplitsa/CSRLab/main/docs/images/mongodb.png" width="20" height="20" alt="mongodb_logo"> to store our data. The structure of the database is basically documents of four types: NGOs and their parameters, parameters of thei social networks pages if there are any, collection of post from each of social media page, and collection of respective comments under those posts if there are any. This is the first version of the schema (which is indicated by `schema_version` parameter), it can be updated later. 

**NGOs collection**

```
{ _id : ObjectId(123),
 ogrn : int,
 <seo parameters>:,
 organisation_name: str,
 hostings_over_time:  [
	{timestamp :, country:, ...},
	{timestamp :, country:, ...},
],
 web_archive_snaps: [
	{timestamp :, snapshot:, ...},
],
 hosting_country_changes: int,
 schema_version: 1,
 social_networks: [
	timestamp: [vk: {}, telegram: {}],
	timestamp: [
			vk: {_id,
				link,
				page_title,
				members,
				diff_members,
			       overall_posts_all_time,
				overall_posts_this_month,
				post_per_month  (keep this value through versions),
mean_comments,
mean_views,
mean_likes,
overall_comments (increment each month),
comments_per_post,
... (all except for the actual texts)
			},
			inst: {_id, link, ...},
			facebook: {_id, link, ...},
			telegram: {_id, link, ...}
		]
]
 ...
}
```

**Social Networks collection**

```
{ _id : ObjectId(123),
 type: vk\inst\tg\fb,
 link: website url,
 org_name: (page_title > official name),
 number_of_posts: >11  (if less use embedding)
 posts: [_post_id,
	     _post_id,
	     ...]
 number_of_comments: >11 (if less use embedding),
 comments: [_comment_id,
		    _comment_id,
		    ...] 
}
```

**Posts collection**

```
{ _id : ObjectId(1234),
 type: vk\inst\fb\tg
 text:,
 media: bool,
 link_to_media: do we want to save it??,
 number_of_likes:,
 number_of_views:,
 number_of_reposts:,
 number_of_comments:,
 comments ???: [_comment_id,
                _comment_id]
 }
```

**Comments collection**

```
{ _id : ObjectId(1234),
 type: vk\inst\fb\tg
 text:,
 media: bool,
 link_to_media:,
 number_of_likes:,
 number_of_replies:,
....
}
```
