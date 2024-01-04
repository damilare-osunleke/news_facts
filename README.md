# news_facts
This project extracts basic info from news articles


before running the script, do the following:
1) if necessary, under section 2, change 'parent_folder' to the path to the parent folder (i.e the folder that contains the news files by country) on your machine  
2) if necessary,under the same section 2, Change "outputs" to the path where you wan to to store your final csv results.

The script works based on the following general assumptions (which hold true for hundreds of files and thousands of news articles tested):
1) files are organised by country. For each country, the folder name is the name of that country. All country folders are inside a folder called 'çountries'
2) files are in RTF format
3) Each article is terminated by a string that starts with the text "Dokument " follwed by the news source (abbreviated e.g DJ for Dow jones), a mix of numerical and alphabetical characters. This string also contains a date in YYYYMMDD format e.g Dokument DJI0000020130819e98j000kj
4) The first paragraph usually has only one line which is written in bold characters. This is the article title. Where the first paragraph has multiple lines, th earticle title is the last line.
5) The date of publishing is always in the second paragraph. It is written in long form with the month in German e.g "12 März 2021"
6) The actual content of the article begins from the 3rd paragraph.
