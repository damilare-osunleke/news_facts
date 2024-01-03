# news_facts
This project extracts basic info from news articles


befor running the script, do the following:
1) create a folder called "countries" (if it doesn't already exist). Add all the news folders (by country) this folder.
2) create a folder "outouts" (if it doesn't already exist) for saving the final output.

The script works based on the follwing general assumptions (which hold true for hundreds of files and thousands of news articles tested):
1) files are organised by country. For each country, the folder name is the nam eof that country. All country folders are inside a folder called 'çountries'
2) files are in RTF format
3) Ech article is terminated by a string that starts with the text "Dokument " follwed by the news source (abbreviated e.g DJ for Dow jones), a mix of numerical and alphabetical characters. This string also contains a date e.g Dokument DJI0000020130819e98j000kj
4) The article title is usually the first paragraph of an article. It is written in bold letters. Where the first paragraph has multiple lines, th earticle title is the last line
5) The date of publishing is always in the second paragraph. It is written in long form with the month in German e.g "12 März 2021"
6) The actual content of the article begins from the 3rd paragraph.
