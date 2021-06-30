### Project Proposal: Linear Regression on_

*Matteo Fortier*
30/06/21

**Framing Question:** What are the most important factors that influence the overall satisfaction rating of a university course? 

Can the satisfaction rating of a university course be modelled with the more specific ratings of the course and/or the options available with a course? (See below for specific feature variables) 

**Purpose and Need:** Universities (in the UK) receive a lot of per course feedback from students via the national student survey, along with an overall satisfaction score for the course. These scores are also publicly available through various websites that help prospecting students choose the universities they want to study at. Consequently, universities have an icentive to keep those overall satisfaction scores high. It is unlikely however, that many universities are able to improve all aspects of a course all at once. Thus it is valuable to model which aspects of a course impacts the overall score the most. 

**Data Description:**

The following data will be scraped:

- Course and rating information. Obtained from: https://discoveruni.gov.uk/course-finder/results/
  - [Example course](https://discoveruni.gov.uk/course-details/10003645/UBSH3BSBS/Full-time/)

There are webpages on 35213 courses (however some lack the data).

Target Variable: Student Satisfaction Rating (Alternatively Average Earnings after 15 months)

Available Feature Variables:

- The teaching on my course ratings (Staff are good at explaining things, Staff have made the subject interesting, The course is intellectually stimulating, My course has challenged me to achieve my best work)
- Learning opportunities ratings (see example page)
- Assessment and feedback ratings (see example page)
- Academic Support ratings (see example page)
- Organisation and management ratings (see example page)
- Learning resources ratings (see example page)
- Learning community ratings (see example page)
- Student voice ratings (see example page)
- Placement year (categorical)
- Year abroad (categorical)

**Tools:**

- Webscrapping via Beautifulsoup. Selenium will also be required for the discoveruni website.
- SQLite database to store the webscrapped data. (Storing as data will be large and time consuming to scrape every time)
- Querying from database into Python via SQLAlchemy
- Regression analysis through Pandas, SciKit and Statsmodels
- Findings will be visualised via matplotlib or seaborn. 

**MVP Goal:**

A potential minimum viable product for the project:

Explore the linear regression model of overall satisfaction rating with one feature. 