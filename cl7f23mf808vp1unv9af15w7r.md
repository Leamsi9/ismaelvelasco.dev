## Is WordPress Killing the Planet?

If you've read my post on [how many emissions are in 1GB](https://ismaelvelasco.dev/emissions-in-1gb) you will know that estimating digital CO2 emissions accurately is a fool's errand. Nevertheless, it is absolutely essential that we do so, not so much to arrive at an absolute measure, but to understand our impact on the environment in a spectrum of evidence based scenarios, and above all, track our direction of travel, and what we need to do to play our part in reducing the painful impacts of climate change.

In this post I will not just look at the emissions of WordPress, but at the size of the internet, how many websites there are, how many of those are active, how many emissions per page, how many per request, and the methodologies behind builtwith.com, W3Techs, Netcraft, Internet Live Stats, and Censys.

So if you're interested in WordPress, digital emissions OR the statistics behind the web, this post is for you.

## TLDR

WordPress is widely said to be used by 40% of websites, and the figure of 455 million sites is frequently repeated. My own estimates below place it much lower, both in total market share and in total websites, but WordPress nevertheless accounts for a gigantic proportion of websites in the world, specially among the 10 million with the highest traffic (as well as the top 100).  This means that out of all CMSs, WordPress has many times more impact on our climate than all other CMS alternatives.  How significant is this carbon footprint?

I estimate that WordPress generates (scope 1) approximately 9000 metric tons of CO2 per day (120 tanker trucks of oil), or 280,000 metric tons of CO2 per month (650,000 barrels of oil), and 3,335,000 metric tons of CO2 per year (the equivalent of razing a forest the size of Beijing every year or adding nearly a million petrol guzzling cars into circulation each year.). Furthermore, the deaths from excess heat of more than 750 of our children and grandchildren in their lifetime will be directly attributable to WordPress. Every year. This does not include WordPress' contribution to deaths from other climate-related consequences, like flooding, food shortages, climate-driven conflict or migration, etc. 

This post explains how I arrived at those figures. It also suggests that the answer to the title question is, sadly, yes, WordPress **is** killing the planet, a little each year.  The good news (yes, there is good news, I'm a utopian realist!), is that it's relatively easy to dramatically cut the CO2 footprint of our WordPress sites, so with modest effort each of us could make a significantly positive impact on the planet. My next post tells you how.


## Estimating WP's CO2 emissions

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1661791511505/qSm6nRGWS.png align="left")

### Minimum estimate
Exact estimations for digital emissions are notoriously elusive, as I said at the start. In an ecosystem as vast and diverse as WordPress, this is even more complex as the emissions from a top 10 website will differ vastly from those of a corner shop.

But we do have some hard numbers to establish a baseline:

#### Emissions per page

The average emissions per webpage is approx. [0.5g of CO2](https://www.websitecarbon.com/). [20 billion WordPress pages are visited each month](https://wordpress.com/activity/).That is around 10,000 metric tons of CO2 per month. 120,000 metric tons per year. 

It would take [planting 2 million trees and growing them for 10 years](https://www.epa.gov/energy/greenhouse-gas-equivalencies-calculator) to compensate for that one year of WordPress. 

The problem is that by then, the emissions would reach over 10 times the accumulated tonnes of CO2. I say more than 10 times because WordPress has been growing at an average annual rathe of 15%, so a decade of emissions woud be closer to 1.5 million tonnes of CO2 (around 20,000 oil tankers of gasoline).  


![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1661791631493/HaiEEvj2C.png align="left")

20,000 oil tankers full of gasoline per year sounds like a lot, but as a metric, it leaves the majority of emissions out. It counts the number of individual page visitors, but not remotely what is going on behind the scenes. Every time you visit that page, there will be trackers, pings, analytics, checks, ads, extensions, spam bots, all sending requests back and forth and generating their own carbon footprint. 

#### Emissions per request

A better metric then is the number of requests, which for WordPress is around [2.6 billion per day](https://www.zdnet.com/article/how-to-optimize-your-site-like-wordpress-com/) (compared to 115 million page views per day to give you an idea of how much more goes on behind the scenes when you visit a webpage). That's 80 billion requests per month. 

Whereas there is a good amount of research on estimated average emissions per web page, there is almost none on average emissions per request. What is clear is that no average is likely to be consistent as the emissions will vary by the amount of data per request; the server and protocol processing requests [Nginx is significantly more efficient than Apache, and HTTP2 better than HTTP1](https://www.researchgate.net/publication/347523090_On_comparing_the_power_usage_of_HTTP11_and_HTTP2_on_webservers); the hosting provider and[hosting zone; and of course the gird intensity at any one time.  You can see how complicated it really gets [here](https://ismaelvelasco.dev/emissions-in-1gb).

One tentative baseline, not as an exact measurement but as a general guide, is comparing the average CO2 per request reported by Google in 2015, and the average CO2 per request calculated in a [2020 Masters Thesis](http://essay.utwente.nl/83631/2/Iseke_MA_EEMCS.pdf) by Ann-Cathrin Iseke. 

Google gives [0.01 kg per request](https://finance.yahoo.com/news/every-google-search-results-co2-090042259.html). Artist Joanna Moll created a sobering page that tells you how many emissions Google.com has generated every second from your landing [here](http://www.janavirgin.com/CO2/). On the one hand, it is likely that the CO2 per request has significantly diminished, as Google implements efficiencies not possible in 2015. For comparison, in 2009 Google estimated 0.2 kg per request, which is 20 times less. By that rate of improvement, Google's emissions would be 0.0005 kg per request in 2021. In fact Google claims to have achieved carbon neutrality,  so these figures would no longer apply, but remain indicative.

Meanwhile, Iseke estimates a range between 0.00013-0.00067 kg of CO2 per request, in the context of the [ArchiSurance](https://www.uio.no/studier/emner/matnat/ifi/INF5120/v18/Resources/archisurance-case-study.pdf) experimental case study for architecture modelling. This matches my estimates for current emissions per request by Google. Taking into account that Google is a benchmark in performance optimisation, and WordPress, alas, is not, it seems safe to assume a notional footprint of 0.0007 kh of CO2 per request to WordPress.com. 

That would mean 1,800 metric tons of CO2 per day, or 56,000 tonnes of CO2 per month, or 670,000 tonnes of CO2 per year. That's over 5 times the emissions from web page visits alone.  This is the equivalent of running almost two gas-fired power plants for a year in the USA. 


![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1661791738845/JNwRszxQM.png align="left")

At the growth rate of 15% WordPress will generate a minimum of 2,345,000 metric tons of CO2 over 10 years, equivalent to the annual electricity consumption of every home in Dubai, and which would require planting 39 million seedlings in 2022 to offset the emissions that would accumulate in the 10 years before they mature into trees. 

Put a different way, running Wordpress sites for 10 years would be the equivalent of cutting down [a forest the size of New York](https://www.epa.gov/energy/greenhouse-gas-equivalencies-calculator).

An even more dramatic  way of putting it is using the mortality cost of carbon (MCC) [proposed in 2021](https://www.nature.com/articles/s41467-021-24487-w) by Daniel Bressler of Columbia University in a widely cited paper in one of the world's top scientific journals, Nature Communications. He puts forward a conservative estimate of the excess deaths from CO2 emissions over the 21st century, in terms of how a release of CO2 emissions now will contribute to global warming over that period. On the current direction of travels he estimates that adding 1 million metric tons of CO2 in 2020 would account for the death of 226 people over that time that would not have occurred had that tonne of emissions not taken place. That would mean that WordPress websites over the next 10 years will be directly responsible for the deaths of at least over 500 of our children and grandchildren, who would not have died without WordPress. 

### Moderate estimate

As a reminder, I described the estimations above as minimal.  The figures don't include the carbon footprint for the [millions of downloads of WordPress itself](https://displaywp.com/wordpress-download-counter/) and its 60,000 plugins. Nor for their storage, and the embodied carbon of their infrastructure.

They don't include the hugely significant emissions of the time spent on a device composing or reading WordPress pages, including battery, electricity, cpu, device life and waste disposal, etc.

But most of all, the data on number of pages and number of requests comes only from sites hosted with WordPress.com and a few others using its Jetpack plugin. Strangely, while Automattic, the owners of WordPress.com, disclose number of pages, of visitors, of requests, of spam blocked, they do not disclose the number of actual websites they host.

I suspect it is because, whereas WordPress core may power 40% of websites according to one metric (see below), WordPress.com only hosts a tiny proportion of these sites. While definite figures are not available to my best knowledge, perhaps a reasonable proxy is the data from BuiltWith.com, according to which they have detected [2 million currently live sites hosted on WordPress.com](https://trends.builtwith.com/cms/WordPress). We could add to those the further [2 million live sites detected as hosted by Automattic](https://trends.builtwith.com/hosting/Automattic). That makes 4 million sites. At the same time, BuiltWith detects 34 million websites using WordPress. 

That would mean that the estimates above represent only 17% of WordPress emissions. 

Adjusting accordingly, we need to augment by 83% the estimates above. That would mean that the likely emissions of WordPress would be a staggering 3.3 million metric tons per year, equivalent to the electricity consumed by every home on Estonia. 

Over 10 years, that would rise to 11.5 million metric tons of CO2, exceeding the annual electricity needs of all of Australia's homes. This means that the next 10 years of WordPress on its current trajectory, will be the equivalent of razing a forest the size of Paris. Twice over.


![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1661791998266/m_ICgj0qe.png align="left")

And it means the death of 2600 of our children and grandchildren from emissions related heat directly attributable to WordPress. 

This may be had to wrap one's head around, but if you're concerned about the accuracy of the figure, it is certain to be an underestimate, as it only accounts for deaths from emissions-related temperature rises, and not from emissions related deaths from infectious disease, climate driven conflict, population displacement, food supply crises, flooding, etc. 

It also doesn't account for the very significant emission-related health impacts short of death for a large proportion of the population. 

### High estimate 

While the moderate estimate relies on figures and ratios from builtwith.com' crawlers and database, popular estimates for the total number of websites running on WordPress range around 455 million, calculated by a [W3Techs estimated market share of 35% for WordPress](https://w3techs.com/blog/entry/40_percent_of_the_web_uses_wordpress) applied a total number of estimated at 1.3 billion websites.

By this reckoning we would have to multiply our moderate estimates by a factor of 12. But thankfully for the environment (maybe not for WordPress?) it's clear that this is a dramatic exaggeration that doesn't take account of either, the methodology used to arrive at the 1.3 billion figure, or that used  to arrive at 35% market share. 


![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1661792220642/hA-FuGJeh.png align="left")

In fact the 1.3 billion figure comes from the [January 2020 Netcraft Server Survey](https://news.netcraft.com/archives/category/web-server-survey/page/6/). Since then we have lost 160 million websites, and the number today stands at [1.1 billion](https://news.netcraft.com/archives/category/web-server-survey/).

The exact methodology and tooling is not, as far as I can tell, fully public, but we can deduce that it relies Internet wide scanning of the IPv4 space, almost certainly using the standard approach of sending a TCP SYN packet to for instance port 80. If the port is closed, the host responds with an RST packet.
If the port is open, the host responds with a TCP SYN/ACK packet indicating that a connection can be established.

So out of all the IP addresses polled this way, 1.1 billion established a connection, indicating a website host in operation. This is the figure given in the many websites promoting the 455 million WordPress sites figure.

There are two problems with this. 

1) Netcraft indicates that "The number of hosts found running internet web sites by the Web Server Survey is large (over 1.1 billion hostnames [August 2022] ), but not exhaustive." 

This suggests that it does not poll the entire IPv4 space, so the actual number of total open hosts is likely to be higher.

This may explain why an equally opaque (as regards specific methods and data sources), but equally authoritative Internet wide counter (cited [by W3C](https://www.w3.org/webat25/news/webfacts) and [by Tim Berners-Lee](https://twitter.com/timberners_lee/status/511988109211627520) among others) has instead found as of August 2022, [1.9 billion websites](https://www.internetlivestats.com/total-number-of-websites/), or nearly double [the current Netcraft figure](https://news.netcraft.com/archives/2022/08/26/august-2022-web-server-survey.html). 

This higher figure is apparently arrived at by integrating a range of data sources (including Netcraft Server Surveys) and projecting second by second estimates using a proprietary [worldometers algorithm (https://www.worldometers.info/about/)]. So again, not an exact number, but a good outer boundary for the total number of sites.

2) The second issue is that open named hosts does not translate into actually active websites. Netcraft estimates that out of the 1.1 billion sites detected, only [200 million sites can be considered active](https://www.netcraft.com/internet-data-mining/). [Internet Live Stats](https://www.internetlivestats.com/total-number-of-websites/) likewise estimated the number of active websites at less that 200 million. The figure may well be derived from []Netcraft itself, and suggests that 70-85% of the web is populated by dead or placeholder websites. 

So if you were to apply the 40% estimated market share to active sites, the figure would go down from the quoted estimate of 455 million to 80 million WordPress sites. This would still require more than doubling the moderate estimate, except for the second flaw in the 455 million calculation. The 40% market share calculated by W3Techs is not calculated from a pool of either 1-2 billion or 200 million websites. Instead it is based on a much more targeted pool of the top 10 million websites as indexed by Alexa. Although Alexa has been retired as a website, [it persists as an API until the end of 2023](https://twitter.com/jdevalk/status/1521748709696061446).

40% of 10 million is 4 million websites, a much smaller figure than the figure detected by builtwith.com. There is no way to say how predictive the market share patterns of the top 10 million sites are of the 190 million remaining active sites, so one cannot credibly apply the market share estimate to the total websites estimates.


### Best estimate

The moderate estimate above relies on builtwith.com's metrics. But there are problems when peering under the hood. BuiltWith affirm that they have [100% coverage](https://builtwith.com/data-coverage) of the web, meaning "domains and subdomains" using "technology under patent", and arrive at a figure of 16.4 billion potential websites. This would be 6 times more than Netcraft's estimates. They define this however as "100% .com/.net/.org & 100% active website coverage".  This is not particularly clear or helpful. It seems to imply that by 100% coverage they mean of those 3 TLDs plus any websites defined as active. I can't tell how that could translate into a 16.4 billion figure, given there are 4.3 billion IPv4 addresses, [614 million registered domains](https://domainnamestat.com/statistics/overview), and 37 (characters allowed) to the power of 63 (maximum characters allowed) potential domain names per TLD, which comes to a 6 followed by 98 zeros, so a lot more than 16.4 billion. Alternatively, there are [189 million domains registered in the .com, .net and .org tlds in August 2022](https://siteefy.com/how-many-domains-are-there/). Each domain can have up to 500 subdomains, but that makes the potential pool 90 billion, not 16.4. It could be that the figure estimates the potential number of virtual hosts for registered domains, or the maximum capacity of detected computers but it's impossible to know.

Similarly, they arrive at a hard to validate figure of 673 million active websites, defined as domains which are not "parked". This is more than 3 times the Netcraft and Internet Live Stats estimates. Given that it is estimated that [around 70% of domains are parked](https://www.glass.ai/glass-news/2019/4/24/70-of-the-internet-isnt-there-and-the-useful-internet-is-smaller-than-we-think), it seems questionable for BuiltWith to arrive at more active websites than registered domains. Adopting the BuiltWith numbers, the market share of WordPress would be 5% of their "non-parked" sites, compared to 40% of the top 10 million sites for W3Techs.  

A more reliable and transparent BuiltWith metric is their total number of websites detected, [which stands at 5.4 million](https://trends.builtwith.com/hosting/traffic/Entire-Internet) as of August 2022. This is closer in line with the 614 million registered domains. Of these, 36% (nearly 2 million websites), cannot resolve the domain, taking down the number to 3.4 million websites. That would give WordPress a 10% global market share, which is probably a better indication than the W3Techs figure. The level of emissions would be the same as in the moderate scenario however, since it has been estimated using BuiltWith's detection figures.  While the total website estimates for BuiltWith appear unreliable, the distributions are credible, given they are built on [a database tracking usage of 60,722+ web technologies over the last 22 years](https://builtwith.com/market-analysis).

One last reliable estimate of the size of the active web can be arrived at via [Censys](https://censys.io/data-and-search/), which uses [zmap](https://zmap.io/) to carry out Internet wide scans of the entire IPv4 space. Its methodology and code are fully open source, and backed by a large body of academic research and tooling extensions. Censys detects 1.9 billion services, 222.5 million hosts and 484.1 million virtual hosts as of August 2022. This aligns much more closely to the 1.9 billion figure from Internet Live Stats quoted above, and the 225 million active hosts is likewise in range for both Internet Live Stats and Netcraft; while the total of 706.6 million hosts plus virtual hosts is in range of the 614 million registered domains, accounting for the fact that Censys scans ports beyond those assigned to http and https, and extends beyond websites only.


![Screenshot 2022-08-29 at 11.54.33.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1661792114628/LrjZGBQ0T.png align="left")


Triangulating the datapoints above, we can take the c. 200 million active sites confirmed by Netcraft, Internet Live Stats and Cesys, and use the 10% BuiltWith market share to arrive at an estimate of 20 million total WordPress sites. That is 5 times more than the number of wordpress.com and automattic sites detected above, which gives us the final multiplier for our baseline, minimal calculations.

My final estimate is that WordPress generates approximately 9000 metric tons of CO2 per day (120 tanker trucks of oil), or 280,000 metric tons of CO2 per month (650,000 barrels of oil), and 3,335,000 metric tons of CO2 per year (a forest the size of Beijing or adding nearly a million cars to annual traffic). On this accounting WordPress will be directly responsible for the deaths from temperature rises of more than 750 of our children and grandchildren in their lifetime. Each year. 

## The Grandparent Effect

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1661792598039/2r6XSXfA6.png align="left")

The above metaphorical tree count should not lead us to lose perspective on the forest itself. Regardless of precise estimate, we can absolutely conclude that WordPress has a significant carbon footprint, which is negatively affecting our planet at scale. Why?

Older CMS providers like WordPress are architected in ways that do not reflect current best practices and would undoubtedly be built differently if starting from scratch today. As an example, WordPress imposes a default paradigm of procedural programming, which makes it less performant, modular, extensible and testable than OOP in PHP 7+. Another example would be lack of native support for package managers like Composer, whereby you can superficially extend the system with plugins, but cannot change or improve it natively with PHP libraries and packages, missing out on the ecosystem of modern PHP programming.  There are ways around this, and several tools and strategies have been developed to make WordPress OOP friendly, and Composer enabled. Furthermore, WordPress has been traditionally hosted on shared or dedicated servers with a CPanel GUI. This has the advantage of dramatically lowering the barriers to entry. It has the disadvantage of not taking advantage of modern web development practices like versioning, continuous integration pipelines, parallel build environments, QA automation, etc.

Again, there are plenty of workarounds, that allow you to build WordPress sites in such modern ways, but they are not the default. 

Then we have the default WordPress database. It is hugely prone to bloat. Every plugin will create its own tables, not tuned or tailored to your specific application. The WordPress revision system, its creaky answer to version control, stores a copy of every draft and update of your blog posts. It is a useful feature as it allows you to revert to older copies of articles and drafts, but it can quickly take up unnecessary space by having no limits on these copies, so you might have a small entry take up one row, and hundreds of redundant copies each with their own row. You would never implement something like this if starting from scratch!

Themes and plugins will also each bring their own data storage strategies, which will often duplicate functionality like logging, capture and accumulate data (specially images) you may never use, and do so in ways you would never approach if you were designing the data layer for an application.  Even when you uninstall them, most will persist their stored data by default, leaving a trail of unused data.

WordPress itself has been actively modernising, for instance by making Headless WordPress possible through an excellent AP, working with cloud providers on improved, WordPress focused, database infrastructure, working to introduce webp formats to reduce image size, and creating a performance team. But such advances still lag enormously behind platforms and approaches built from scratch in the last 5 years, from JamStack to developer friendly CMSs like Statamic, built on Laravel. These are natively much easier to scale, customise and extend than WordPress after all the workarounds.


## The opportunity: be the change you want to see

Does that mean we should all abandon WordPress for more modern, more environmentally friendly systems? This would hardly be realistic, given the millions of sites already running on WordPress, and its remarkable ecosystem, although there are signs that in the last couple of years, for the first time, [people are indeed leaving WordPress](https://joost.blog/wordpress-market-share-shrinking/) for more performant (therefore likely greener) alternatives.

But from the point of view of climate change, at the present adoption rates, reducing the carbon footprint of the WordPress ecosystem would be far more impactful and beneficial for the planet than advocating for greener alternatives with a fraction of adoption. Of course both approaches are complementary. Refining and diversifying the tools available for climate friendly website development is crucial. But greening the existing ecosystem is just as important.

In this sense, the good news for people working with WordPress, is that they are in a position to have a greater impact by dedicating their energies to greening WordPress (not just their own sites) than by simply switching CMS platforms. The other good news is that we have already developed a wealth of design patterns, tools and workarounds to turn WordPress into a highly performant, highly energy efficient engine. Finally, by greening WordPress they also improve its performance, meaning the loss of market share my be halted or even reversed, which, if WordPress became a force for emission reductions, would only be good news.

As one example of what's possible, I leave you with the [sustyweb](https://sustywp.com/] WordPress theme, which managed to create a fully working theme that runs on 6kb. This could be a good foundation to build from, adopting and adapting [the underlying design principles](https://css-tricks.com/delivering-wordpress-in-7kb/) to our own websites. I am not advocating your website should look like that team, but that by adding whatever you are missing in a minimalist way, you can be confident of building the most climate friendly WordPress site possible that still fulfils your use case needs.
