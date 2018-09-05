# RPHA_DataLeecher
Web Scraper for getting data from periodicals in the online archives of Hungary's National Széchényi Library, using BeautifulSoup and nltk. 

Structure for the websites is:
- Site A is the only input needed. It is a list of all issues of the periodical, pointing to:
- Site B's, which are lists of works in the specific issue, pointing to:
- Site C's, which are the works themselves.

Info it can get:
- Year and month of issue in which work was first published (from site B's)
- Name of author (from site B's)
- Gender of author - done by checking name against lists of male and female names (from site B's)
- Title of work (from site B's)
- Incipit (beginning sentence(s)) of work - getting sentences was done using nltk (from site C's)
- Genre of work (from HTML tags on site C's)
- Link pointing to work's online version (from site B's).

The result is an HTML table that can be directly copied into an Excel spreadsheet.


Hastily done in a few days with no prior knowledge of Python, relying on tutorials and a basic understanding of programming concepts since I already knew some JS.

Based on an estimate, this code saved me about two months of not-so-exciting manual copying, getting data from a total of some 25,000 works.
