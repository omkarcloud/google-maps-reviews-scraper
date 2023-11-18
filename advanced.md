## 🤔 Advanced Questions

### ❓ I don't have Python, or I'm facing errors when setting up the scraper on my PC. How to solve it?

You can easily run the scraper in Gitpod, a browser-based development environment. Set it up in just 5 minutes by following these steps:

1. Sign up using your GitHub account at [this link](https://gitpod.io/#https://github.com/omkarcloud/google-maps-scraper).
   
   ![Screenshot (148)](https://github.com/omkarcloud/google-maps-scraper/assets/53407137/f498dda8-5352-4f7a-9d70-c717859670d4.png)
  
2. Once signed up, open it in Gitpod.   

   ![gp-continue](https://raw.githubusercontent.com/omkarcloud/google-maps-reviews-scraper/master/screenshots/gp-continue.png)

3. Paste the following code into `main.py`:
```python
from src.gmaps import Gmaps
star_it = '''Love It? Star It! ⭐ https://github.com/omkarcloud/google-maps-reviews-scraper/'''

queries = ["web developers in bangalore"]
Gmaps.places(queries, scrape_reviews=True, max=5)
```

4. To start scraping, execute this command in the terminal:
   ```bash
   python main.py
   ```
  
5. After the scraper finishes, download the leads from the `output` folder.

   ![Google Maps Reviews Scraper Result Sample](https://raw.githubusercontent.com/omkarcloud/google-maps-reviews-scraper/master/screenshots/google-maps-reviews-scraper-result.png)

Configure the scraper in Gitpod as you would locally by editing the `main.py` file and running the scraper with the `python main.py` command.

Remember to interact with the Gitpod environment, like clicking within it every 30 minutes, to keep the machine active and prevent automatic shutdown. 

If you prefer not to click every 30 minutes, consider installing Python on your PC and running the scraper locally.

### ❓ Does running Scraper on Bigger Machine scrapes Data Faster?

No, the scraper is resource-light, showing no significant speed difference whether it's run on an Intel Pentium processor with 4GB of RAM or an Intel i7 processor with 16GB of RAM.

### ❓ How to select more fields?

Seeing a lot of fields can be intimidating, so we have only kept the most important fields in the output for places. You can choose from up to 45+ fields.

To select all fields, use the code below:
```python
queries = [
   "web developers in bangalore"
]
Gmaps.places(queries, scrape_reviews=True, max=5, fields=Gmaps.ALL_FIELDS)
```

For specific fields only, use this code:
```python
queries = [
   "web developers in bangalore"
]

fields = [
   Gmaps.Fields.PLACE_ID, 
   Gmaps.Fields.NAME, 
   Gmaps.Fields.MAIN_CATEGORY, 
   Gmaps.Fields.RATING, 
   Gmaps.Fields.REVIEWS, 
   Gmaps.Fields.WEBSITE, 
   Gmaps.Fields.PHONE, 
   Gmaps.Fields.ADDRESS,
   Gmaps.Fields.LINK, 
]

Gmaps.places(queries, scrape_reviews=True, max=5, fields=fields)
```

Note: The number of selected fields does not impact scraping time.

### ❓ How to Change the Language of Output?
Pass the `lang` argument. For example, to scrape results in Spanish, use `lang="Gmaps.Lang.Spanish"`.

```python
queries = [
   "web developers in bangalore"
]
Gmaps.places(queries, scrape_reviews=True, max=5, lang=Gmaps.Lang.Spanish)
```

All Google Maps languages are supported. Some popular languages you may want to use are:
- Gmaps.Lang.Spanish
- Gmaps.Lang.English
- Gmaps.Lang.Japanese
- Gmaps.Lang.German
- Gmaps.Lang.Italian

See the full list of supported languages [here](https://github.com/omkarcloud/google-maps-reviews-scraper/blob/master/languages.md).

**Note:** The `published_at_date` and `response_from_owner_date` fields are provided only in English. They will be null if you scrape reviews in other languages.

### ❓ I have Google Map Places Links, How to Scrape Links?

Utilize the `links` method to extract information from specific Google Maps place links. Here’s an example:

```python
links = [
   "https://www.google.com/maps/place/Zinavo-+Web+Development,+Web+Design+Company+in+Bangalore,+SEO+Services,+Digital+Marketing+Agency,+eCommerce+Web+Development/@13.01443,77.6480612,17z/data=!3m1!4b1!4m6!3m5!1s0x3bae172f3e7069f1:0xbcac5b2d393c2aa2!8m2!3d13.01443!4d77.6480612!16s%2Fg%2F11h0l3y9l?authuser=0&hl=en&entry=ttu",
   "https://www.google.com/maps/place/SeekNEO+-+Web+Development,+Web+Design+Company+in+Bangalore,+eCommerce+Web+Development,+SEO+Services,+Digital+Marketing+Agency/@12.9863763,77.5473899,17z/data=!3m1!4b1!4m6!3m5!1s0x3bae13ac4bcc6641:0x1bf48a7dee3d5a51!8m2!3d12.9863763!4d77.5473899!16s%2Fg%2F11g2338zrl?authuser=0&hl=en&entry=ttu"
]
output_folder = "my-awesome-places"

Gmaps.links(links, output_folder, scrape_reviews=True, max=5)
```

### ❓ Do I Need Proxies?

No, proxies are not necessary. The scraper can efficiently process hundreds of thousands of leads without them.

### ❓ What is the Difference Between your google-maps-scraper and google-maps-reviews-scraper?

Both repositories use the same web scraper but are tailored for different audiences:

**omkarcloud/google-maps-reviews-scraper:** 
- Designed for Data Scientists.
- Its README focuses on scraping reviews for sentiment analysis.

**omkarcloud/google-maps-scraper:** 
- Aimed at Entrepreneurs.
- Its README focuses on extracting business listings for lead generation.

**Choose based on your need:**
- Data Scientists for sentiment analysis ➡️ `google-maps-reviews-scraper`, as its README is written specifically for your use case.
- Entrepreneurs for leads ➡️ `google-maps-scraper`, as its README is written specifically for your use case.


Note: Both repositories are exactly same in terms of code and functionality. The only difference is the README.

### ❓ I am a Web Scraper; The Scraper is Really Impressive with Caching and Parallel Scraping Features?

Yes, it includes advanced features that enhance efficiency and user experience, such as:

- Parallel scraping to save time.
- Keeping drivers alive for quick task initiation.
<!-- - Automatic calculation of the number of scrapers to run in parallel based on system resources. -->
- Asynchronous scraping, allowing for data scraping in the background.
- Caching results so you can pick up where you left off in case of interruption.

The scraper leverages the Botasaurus Web Scraping Framework, which simplifies the implementation of these features. We encourage you to learn about the Botasaurus Framework to save countless hours in your career as a web scraper, [here](https://github.com/omkarcloud/botasaurus).

<p align="center">
  <a href="https://github.com/omkarcloud/botasaurus">
  <img src="https://raw.githubusercontent.com/omkarcloud/botasaurus/master/images/mascot.png" alt="botasaurus" />
</a>
</p>

## Love It? [Star It ⭐!](https://github.com/omkarcloud/google-maps-reviews-scraper)

Become one of our amazing stargazers by giving us a star ⭐ on GitHub!

It's just one click, but it means the world to us.

[![Stargazers for @omkarcloud/google-maps-reviews-scraper](https://bytecrank.com/nastyox/reporoster/php/stargazersSVG.php?user=omkarcloud&repo=google-maps-reviews-scraper)](https://github.com/omkarcloud/google-maps-reviews-scraper/stargazers)