![Google Maps Scraper Feautred Image](https://raw.githubusercontent.com/omkarcloud/google-maps-reviews-scraper/master/screenshots/google-maps-reviews-scraper-feautred-image.png)

<div align="center" style="margin-top: 0;">
  <h1>✨ Google Maps Scraper 🤖</h1>
</div>
<em>
  <h5 align="center">(Programming Language - Python 3)</h5>
</em>
<p align="center">
  <a href="#">
    <img alt="google-maps-scraper forks" src="https://img.shields.io/github/forks/omkarcloud/google-maps-scraper?style=for-the-badge" />
  </a>
  <a href="#">
    <img alt="Repo stars" src="https://img.shields.io/github/stars/omkarcloud/google-maps-scraper?style=for-the-badge&color=yellow" />
  </a>
  <a href="#">
    <img alt="google-maps-scraper License" src="https://img.shields.io/github/license/omkarcloud/google-maps-scraper?color=orange&style=for-the-badge" />
  </a>
  <a href="https://github.com/omkarcloud/google-maps-scraper/issues">
    <img alt="issues" src="https://img.shields.io/github/issues/omkarcloud/google-maps-scraper?color=purple&style=for-the-badge" />
  </a>
</p>
<p align="center">
  <img src="https://views.whatilearened.today/views/github/omkarcloud/google-maps-scraper.svg" width="80px" height="28px" alt="View" />
</p>

<p align="center">
  <a href="https://gitpod.io/#https://github.com/omkarcloud/google-maps-scraper">
    <img alt="Open in Gitpod" src="https://gitpod.io/button/open-in-gitpod.svg" />
  </a>
</p>
  
---

## Disclaimer for Google Maps Scraper Project

> This Google Maps Scraper is provided for educational and research purposes only. By using this Google Maps Scraper, you agree to comply with local and international laws regarding data scraping and privacy. The authors and contributors are not responsible for any misuse of this software. This tool should not be used to violate the rights of others, for unethical purposes, or to use data in an unauthorized or illegal manner.

We take the concerns of the Google Maps Scraper Project very seriously. For any concerns, please contact Chetan Jain at [chetan@omkar.cloud](mailto:chetan@omkar.cloud). We will promptly reply to your emails.

##  Explore Our Other Awesome Products

- ✅ [BOTASAURUS](https://github.com/omkarcloud/botasaurus): The All-in-One Web Scraping Framework with Anti-Detection, Parallelization, Asynchronous, and Caching Superpowers.

<!-- - ✅ [GOOGLE SCRAPER](https://github.com/omkarcloud/google-scraper): Discover Search Results from Google. -->

<!-- - ✅ [AMAZON SCRAPER](https://github.com/omkarcloud/amazon-scraper): Discover Search Results and Product Data from Amazon. -->

<!-- - ✅ [TRIP ADVISOR SCRAPER](https://github.com/omkarcloud/tripadvisor-scraper): Discover search results of hotels and restaurants from TripAdvisor. -->

---

Google Maps Scraper helps you find Business Profiles from Google Maps.

## ⚡ Benefits

1. Easy-to-use, friendly dashboard.

2. Limitless scraping: Say sayonara to costly subscriptions or expensive pay-per-result fees.

3. Highly scalable, capable of running on Kubernetes, Docker, and servers.

4. Scrape data for a specific type of business across all cities in a country.

5. Get the exact results you need by easily sorting, filtering, and exporting data as CSV, Excel, or JSON files.

6. Scrape reviews while ensuring the privacy of reviewers is maintained.

In the next 5 minutes, you'll extract **120 Search Results** from Google Maps.

![Google Maps Data Scraper CSV Result](https://raw.githubusercontent.com/omkarcloud/google-maps-scraper/master/screenshots/gmap_result.png)

## 📦 Requirements

To use this tool, you'll need:

- Node.js version 16 or later to run the UI Dashboard (please check your Node.js version by running `node -v`)
- Python for running the scraper

**Don't have Node.js or Python? No problem!**  

You can easily run this tool within Gitpod, a cloud-based development environment. We'll cover how to set that up later. 

## 🚀 Getting Started

Let's get started by following these super simple steps:

1️⃣ Clone the Magic 🧙‍♀️:
```shell
git clone https://github.com/omkarcloud/google-maps-scraper
cd google-maps-scraper
```

2️⃣ Install Dependencies 📦:
```shell
python -m pip install -r requirements.txt && python run.py install
```

3️⃣ Launch the UI Dashboard 🚀:
```shell
python run.py
```

4️⃣ Open your browser and go to [http://localhost:3000](http://localhost:3000), then press the Run button to have 120 search results within 2 minutes. 😎

![GIF of Google Maps Scraper Visit, Highlish Keyword, Run, See Results](https://raw.githubusercontent.com/omkarcloud/google-maps-scraper/master/screenshots/demo.gif)

*Note: If you don't have Node.js 16+ and Python installed or you are facing errors, follow this Simple FAQ [here](https://github.com/omkarcloud/google-maps-reviews-scraper/blob/master/advanced.md#-i-dont-have-python-or-im-facing-errors-when-setting-up-the-scraper-on-my-pc-how-to-solve-it), and you will have your search results in the next 5 Minutes*

## ⚡ Enlightening Questions

### ❓ How to Get Results for My Queries?

1. Visit [http://localhost:3000](http://localhost:3000) and enter your search queries.

![Queries](https://raw.githubusercontent.com/omkarcloud/google-maps-scraper/master/screenshots/queries.png)

2. Now, simply press the Run button.

![Run](https://raw.githubusercontent.com/omkarcloud/google-maps-scraper/master/screenshots/run.png)

### ❓ What are the different pages and how do they help me?

Primarily, there are 3 pages in the UI Dashboard:

- Home Page ('/')
- Output Page ('/output')
- Results Page ('/output/1')

#### Home Page ('/')

![Homepage](https://raw.githubusercontent.com/omkarcloud/google-maps-scraper/master/screenshots/homepage.png)

You can input your queries here and search by:
- List of queries
![Queries](https://raw.githubusercontent.com/omkarcloud/google-maps-scraper/master/screenshots/queries.png)

- Scrape data for a specific type of business across all cities in a country.
![country-section](https://raw.githubusercontent.com/omkarcloud/google-maps-scraper/master/screenshots/country-section.png)

- Scrape Reviews
![reviews-section](https://raw.githubusercontent.com/omkarcloud/google-maps-scraper/master/screenshots/reviews-section.png)

#### Output Page ('/output')
![output-page.png](https://raw.githubusercontent.com/omkarcloud/google-maps-scraper/master/screenshots/output-page.png)

The Output page helps you manage your tasks. You can use it to:

- See tasks and their status (pending, in progress, or completed).
- Abort or delete any task.
![abort-delete.png](https://raw.githubusercontent.com/omkarcloud/google-maps-scraper/master/screenshots/abort-delete.png)

- Additionally, Whenever you run a query, a task named "All Task" will be created for it, which combines results from multiple queries.

For example, if you search for "Web Developers in Bangalore" and "Web Developers in Mumbai", the "All Task" will show you the combined results for both queries.

![all-task.png](https://raw.githubusercontent.com/omkarcloud/google-maps-scraper/master/screenshots/all-task.png)

#### Results Page ('/output/1')
![results-page.png](https://raw.githubusercontent.com/omkarcloud/google-maps-scraper/master/screenshots/results-page.png)

This is the most important page where you can view, sort, filter, or download the results of the task.

**Sorting**

![sort.png](https://raw.githubusercontent.com/omkarcloud/google-maps-scraper/master/screenshots/sort.png)

You can also sort by other criteria, such as name or reviews.

![sort-small.png](https://raw.githubusercontent.com/omkarcloud/google-maps-scraper/master/screenshots/sort-small.png)

**Filters**

![filter.png](https://raw.githubusercontent.com/omkarcloud/google-maps-scraper/master/screenshots/filter.png)

To find the exact results you're looking for, click the "Show Filters" button and apply the desired filters.

**Export**

![export.png](https://raw.githubusercontent.com/omkarcloud/google-maps-scraper/master/screenshots/export.png)

Download results in various formats (CSV, JSON, Excel) using the export button.

### ❓ Where is the Code for the Scraper?
Kindly find the complete code at [omkarcloud/google-maps-scraper](https://github.com/omkarcloud/google-maps-scraper)

### ❓ This Scraper is Truly One-of-a-Kind, Something I've Never Seen Before. How Did You Build It?

Thank you! We used Botasaurus, which is the secret behind our awesome Google Maps Scraper.

Botasaurus is a web scraping framework that makes life a lot easier for web scrapers.

It handled the hardest parts of our scraper, such as:

- Creating a gorgeous UI dashboard with task management features
- Sorting, filtering, and exporting data as CSV, JSON, Excel, etc.
- Caching, parallel and asynchronous scraping, and anti-detection measures
- Built-in integration with Kubernetes, Docker, Server, Gitpod, and a REST API

If you're a web scraper, I really recommend learning about Botasaurus [here 🚀](https://github.com/omkarcloud/botasaurus).

Trust me, learning Botasaurus will only take 20 minutes, but I guarantee it will definitely save you thousands of hours in your life as a web scraper.

<p align="center">
  <a href="https://github.com/omkarcloud/botasaurus">
    <img src="https://raw.githubusercontent.com/omkarcloud/botasaurus/master/images/mascot.png" alt="botasaurus" />
  </a>
</p>

### ❓ Advanced Questions

Having read this page, you have all the knowledge needed to effectively use the tool.

You may choose to read the following questions based on your interests:

1. [I Don't Have Python, or I'm Facing Errors When Setting Up the Scraper on My PC. How to Solve It?](https://github.com/omkarcloud/google-maps-reviews-scraper/blob/master/advanced.md#-i-dont-have-python-or-im-facing-errors-when-setting-up-the-scraper-on-my-pc-how-to-solve-it)
2. [Do I Need Proxies?](https://github.com/omkarcloud/google-maps-reviews-scraper/blob/master/advanced.md#-do-i-need-proxies)
3. [What is the Difference Between your google-maps-scraper and google-maps-reviews-scraper?](https://github.com/omkarcloud/google-maps-reviews-scraper/blob/master/advanced.md#-what-is-the-difference-between-your-google-maps-scraper-and-google-maps-reviews-scraper)

### ❓ Need More Help or Have Additional Questions?

For further help, feel free to reach out to us through:

- **WhatsApp:** If you prefer WhatsApp, simply send a message [here](https://api.whatsapp.com/send?phone=918295042963&text=Hi,%20I%20would%20like%20to%20learn%20more%20about%20your%20products). Also, to help me provide the best possible answer, please include as much detail as possible.

  [![Contact Us on WhatsApp about Google Maps Scraper](https://raw.githubusercontent.com/omkarcloud/assets/master/images/whatsapp-us.png)](https://api.whatsapp.com/send?phone=918295042963&text=Hi,%20I%20would%20like%20to%20learn%20more%20about%20your%20products)


- **GitHub Discussions:** If you believe your question could benefit the community, feel free to post it in our GitHub discussions [here](https://github.com/omkarcloud/google-maps-scraper/discussions).

  [![Contact Us on GitHub Discussion](https://raw.githubusercontent.com/omkarcloud/google-maps-scraper/master/screenshots/ask-on-github.png)](https://github.com/omkarcloud/google-maps-scraper/discussions)

- **Email:** If you prefer email, kindly send your queries to [chetan@omkar.cloud](mailto:chetan@omkar.cloud). Also, to help me provide the best possible answer, please include as much detail as possible.

  [![Contact Us on Email about Google Maps Scraper](https://raw.githubusercontent.com/omkarcloud/google-maps-scraper/master/screenshots/ask-on-email.png)](mailto:chetan@omkar.cloud)

We look forward to helping you and will respond to emails and whatsapp messages within 24 hours.

Good Luck!

## Love It? [Star It ⭐!](https://github.com/omkarcloud/google-maps-reviews-scraper)

Become one of our amazing stargazers by giving us a star ⭐ on GitHub!

It's just one click, but it means the world to me.

[![Stargazers for @omkarcloud/google-maps-reviews-scraper](https://bytecrank.com/nastyox/reporoster/php/stargazersSVG.php?user=omkarcloud&repo=google-maps-reviews-scraper)](https://github.com/omkarcloud/google-maps-reviews-scraper/stargazers)


## Made with ❤️ using [Botasaurus Web Scraping Framework](https://github.com/omkarcloud/botasaurus)
