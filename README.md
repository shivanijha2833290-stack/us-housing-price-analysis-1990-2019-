# us-housing-price-analysis-1990-2019-
A Power BI dashboard exploring how interest rates, inflation, and bank credit availability drove US home price growth from 1990 to 2019.
# backstory 
This project actually started life as an econometrics assignment in my 4th
semester. Back then, I understood the economic theory behind it but didn't
know Power BI or Python well enough to actually build the analysis I had in
mind, so it stayed as notes and half-finished ideas.

I later went back, learned Power BI properly, and rebuilt the whole thing
from scratch — this is the result, and my first dashboard ever. Sharing it
here both as a portfolio piece and as a reminder to my future self that it's
fine to revisit something you couldn't finish the first time around.
Download `us_housing_price_analysis.pbit`<img width="1336" height="747" alt="us housing price analysis (1990-2019)" src="https://github.com/user-attachments/assets/0e2bde23-c063-4e24-b6a1-7062134cab8c" />
# insights :
**Interest rates vs. home prices** — an inverse relationship: as borrowing
costs fell, housing demand and prices rose.
**Inflation vs. home prices** — in the 1990s, everyday prices (inflation)
rose quickly while homes stayed cheap. After 2000, inflation cooled off but
home prices kept climbing — general inflation wasn't what made homes harder
to afford.
**Bank credit vs. home prices** — as banks extended more credit over the
years, home prices rose in tandem, showing that easier access to borrowed
money pushed up demand and prices.
**Prices by era** — the Recovery period holds the largest share of total
home price growth, followed by the Recession era (~34.6%), showing the
market rebounded strongly after the crash
# conclusion: Falling interest rates led banks to extend more credit, and
even as inflation cooled, cheap borrowed money kept pushing home prices
higher — peaking during the post-2011 recovery. This suggests easy access to
credit, not inflation or the broader economy alone, was the primary driver
of rising US home prices.
# data model 
Single table (`sample data`) with the following fields:
Column	Type	Description
`**year	Integer	Calendar year (1990–2019)
`median sales price (usd)`	Currency	Median US home sales price
`average federal interest rate`	Decimal	Average federal funds interest rate
`inflation rate`	Decimal	Annual inflation rate
`total bank credit`	Decimal	Total outstanding bank credit
`era`	Text	Economic period label (e.g., Recession, Recovery)
# dax measures 
`median home price` — sum of median sales price
`bank credit` — sum of total bank credit
`credit yoy growth` — year-over-year % change in bank credit
`credit growth from 1990 %` — % growth in bank credit relative to the 1990 baseline
`total median price` — sum of median sales price
# data source
data.gov.in
world bank data 
# how to use 
Download `us_housing_price_analysis.pbit`
Open it in Power BI Desktop (free download from Microsoft)
When prompted, either connect it to your own data source in the same
format, or load the included sample dataset
Explore the interactive filters and drill into any era or year range
# tools used
Power BI Desktop
Power Query (data shaping)
DAX (measures & calculated fields)
# author 
shivani jha 
linkdin url:https://www.linkedin.com/in/shivanijha0?utm_source=share_via&utm_content=profile&utm_medium=member_android


