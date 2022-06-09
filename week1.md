On this week I installed software that I will use for this course. My
choise is RStudio. I know better how to work in SPSS, even though I have
experience in both software. However I want to advance my knowlage in R
rather than in SPSS.

There were no any problems installing RStudio since I had already had
it.  
Data was downloaded from:
<https://www.europeansocialsurvey.org/download.html?file=ESS9e03_1&y=2018>  
Codebook fro the data can be found by the following link:
<chrome-extension://efaidnbmnnnibpcajpcglclefindmkaj/viewer.html?pdfurl=https%3A%2F%2Fwww.europeansocialsurvey.org%2Fdocs%2Fround9%2Fsurvey%2FESS9_appendix_a7_e03_1.pdf&clen=2111156>

The European Social Survey (ESS) is an academically-driven multi-country
survey, which has been administered in over 35 countries to date. Its
three aims are, firstly – to monitor and interpret changing public
attitudes and values within Europe and to investigate how they interact
with Europe’s changing institutions, secondly – to advance and
consolidate improved methods of cross-national survey measurement in
Europe and beyond, and thirdly – to develop a series of European social
indicators, including attitudinal indicators. For the course we will use
round 9 ESS.

Variables of the datases are separated for the following groups:  
Country  
Weights  
Media and social trust  
Politics  
Subjective well-being, social exclusion, religion, national and ethnic
identity  
Timing of life  
Gender, Year of birth and Household grid  
Socio-demographics  
Justice and Fairness  
Human values  
Administrative variables  
Sample Design variables  
User defined variables

While imporing the dataset I got a problem that most likley is a
begginer problem: the available datasets were just for SPSS, SAS, STATA.
I downloaded and opened data in SPSS and chnaged the file type for
“.csv”. The rest of the work was familiar for me. Aftr importing data, I
had a look at the dataset and it looked good. Then, I saved tha data to
the folder. Initially I wanted to save it in “.csv” format, but after i
saw that “.rda” format was used by teacher. I googled and used rda
format since the data file is huge and it will makw thw loading process
faster, Here is a link where i found out the difference between the
formats:
<https://stackoverflow.com/questions/58699848/best-file-type-for-loading-data-in-to-r-speed-wise>.

    setwd("C:/R scripts/DWA2022")
    data <- read.table("C:/R scripts/DWA2022/ESS9e03_1.csv", header=T, sep = ';')

    View(data)

    save(data,file="data.Rda")
