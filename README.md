# IMDB Top 250 Movies — Power BI Dashboard 🎬

Interactive analysis of the **IMDB Top 250 Movies** using Power BI.  
Focus areas: ratings distribution, decades, genres, and directors.

## Data Source
- Source page: [IMDB Top 250 Movies](https://www.imdb.com/chart/top)  
- Data was **loaded directly from the web** using **Power BI’s Web connector** and cleaned in **Power Query**.  
- No raw CSV/Excel is included in this repo to respect IMDB’s terms; instead, the source link and steps to recreate are provided.


## Transformations (Power Query)
- Parsed movie title, year, and rating from the web table
- Split “Title (Year)” into separate **Title** and **Year**
- Extracted **Decade** from Year (e.g., 1994 → 1990s)
- Trimmed/cleaned text fields, removed duplicates and nulls
- (Optional) Mapped or split **Genres** where available

## Features
- ⭐ KPIs: Highest-rated film, Average rating, Record count
- 📊 Ratings distribution (histogram)
- 📅 Movies by **Decade**
- 🎭 Movies by **Genre**
- 🎬 Top directors with multiple entries

## Files in this repo
- `IMDB_Top250_Dashboard.pbix` — Power BI report
- `images/` — dashboard screenshots

## Preview
![Dashboard Overview](images/dashboard1.png)
![Directors & Decades](images/dashboard2.png)

## Recreate the dataset (Power BI)
1. **Home → Get Data → Web**
2. Paste the URL: `https://www.imdb.com/chart/top`
3. In the Navigator, pick the table that lists the Top 250 (the main results table)
4. Click **Transform Data** → apply the cleaning steps above in **Power Query**
5. **Close & Apply** → build visuals

## How to use
- Download the `.pbix`
- Open in **Power BI Desktop**
- Explore filters, drilldowns, and pages

## Attribution
- Data © IMDB — used here **for educational/portfolio purposes**.  
- This repo does **not** redistribute IMDB data files; it documents the analysis and links to the public source page.
