Scrape Facebook posts with comments from one or multiple page URLs. Get post and comment texts, timestamps, page and post URLs, likes, shares, followers and comments count, author IDs, and more. Download data in structured formats such as JSON, CSV, XML, Excel, and HTML and use it in apps, spreadsheets, and reports.


## Why scrape Facebook posts? 

Our free Facebook Posts Scraper allows scraping the most recent posts (with or without comments) from one or multiple chosen Facebook pages. Scraping the most recent Facebook posts can automate data collection to spot shifts in customer attitudes, analyze social media phenomena and their influence, identify hot spots of misinformation, fake news, hate speech, and more.

If you are unsure how your business or project could use the data scraped from Facebook posts, you can browse through our [industries pages](https://apify.com/industries)  for ideas and use cases.

## How to scrape Facebook posts

Facebook Posts Scraper has an approachable UI, so there aren't too many scraping parameters to set.

1.  [Create](https://console.apify.com/sign-up)  a free Apify account.
2.  Open  [Facebook Latest Posts Scraper](https://apify.com/pocesar/facebook-latest-posts-scraper)
3.  Add one or more Facebook page URLs to scrape its most recent posts and comments.
4.  Click *Run* and wait for the datasets to be extracted.
5.  Download your data in JSON, XML, CSV, Excel, or HTML.


## Want to scrape Facebook comment section?

If you need to make your scraping more specific and get comments from chosen posts, consider trying this mini-scraper's twin - [Facebook Comments Scraper](https://apify.com/pocesar/facebook-latest-comments-scraper). Our mini-scrapers are designed in such a way that just 1 or 2 inputs are enough to get quick results. Just enter one or more page URLs and click to start the scraping. 


## Need something more advanced?

Try our more advanced [Facebook Pages Scraper](https://apify.com/pocesar/facebook-pages-scraper) or [Facebook Ads Scraper](https://apify.com/tugkan/facebookads-scraper) if you need a wider array of options and are comfortable with configuring various scraper settings on your own.

Also, let us know if you need a [custom Facebook scraping solution](https://apify.com/custom-solutions).

##   Cost of usage

Based on Apify's pricing at the time of writing, the Personal plan **($49)** would allow you to scrape about: 
-   20-30k posts monthly **without comments**
-   10-20k posts monthly **including comments**

To run this actor, you will need to have access to [residential proxies](https://apify.com/proxy). If you don't already have access, contact us at [support@apify.com](mailto:support@apify.com).

For more info on how the price for scraping Facebook is formed, read in [Cost of usage](https://apify.com/pocesar/facebook-pages-scraper#cost-of-usage) of the main Facebook Pages Scraper.


## Input


Here's an example input for scraping a few posts from a Facebook page, **without** comments. It has only one required parameter - **startUrls**. To scrape comments to the posts as well, just enable the optional parameter **includeLastComments**. You can check the `INPUT_SCHEMA` tab for more details.

```javascript
{  
	"startUrls":  [  
		{  
			"url": "https://www.facebook.com/ScienceMagazine"
		}  
	],
	"includeLastComments":  false  
}
```

## Output

This mini-scraper will deliver results in a dataset. You can choose in which format to download it: JSON, Excel, HTML CSV, or XML. Here's an excerpt from the JSON dataset you'd get if you apply the input parameters above:
```json
{
  "author": "Science",
  "fbPage": "https://www.facebook.com/ScienceMagazine/",
  "site": "https://www.science.org/",
  "profile": "Science",
  "postText": "How massive is that supermassive black hole? \n\nNew research in Science provides a novel method for characterizing the masses of these entities. Read more ➡ https://fcld.ly/ogtt666",
  "postUrl": "https://www.facebook.com/ScienceMagazine/videos/374163854432473/",
  "date": "2021-08-17T19:30:02.000Z",
  "modifiedDate": "2021-09-12T13:08:41.000Z",
  "imageCaption": null,
  "imageUrl": null,
  "likesCount": 421,
  "sharesCount": 65,
  "commentsCount": 7,
  "followerCount": 4565309,
  "thumbnailUrl": null,
  "comments": []
}
{
  "author": "Science",
  "fbPage": "https://www.facebook.com/ScienceMagazine/",
  "site": "https://www.science.org/",
  "profile": "Science",
  "postText": "Watch to learn how fossil apes have strengthened ideas about how humans evolved, and what steps we can take to learn even more about our ancient ancestors. https://fcld.ly/v4z106n",
  "postUrl": "https://www.facebook.com/ScienceMagazine/videos/355106916040972/",
  "date": "2021-05-22T18:00:09.000Z",
  "modifiedDate": "2021-07-26T16:33:48.000Z",
  "imageCaption": null,
  "imageUrl": null,
  "likesCount": 914,
  "sharesCount": 86,
  "commentsCount": 29,
  "followerCount": 4565309,
  "thumbnailUrl": null,
  "comments": []
},
...
```

## Limitations

-   No login support.
- Does not scrape replies yet, only comments.
-   The "About" page can't be accessed publicly.
-   No content, stats, or comments for live stream posts.
-   The order of items isn't necessarily the same as seen on the page and is not sorted by date.

## Personal data

We do not consider scraping vast amounts of personal data ethical and discourage anyone from doing so. Facebook Posts Scraper **does not scrape personal data from profiles**, including emails, addresses, phone numbers, etc. 
Personal data is protected by GDPR in the European Union and other laws and regulations around the world. You should not scrape it unless you have a legitimate reason to do so. If you're unsure whether your reason is legitimate, consult your lawyers. Please read our blog post about  [creating ethical and compliant scrapers](https://blog.apify.com/is-web-scraping-legal/)  if you would like to learn more.
