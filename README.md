# Acces-web-data-with-python-Beautiful-Soup-timesjobs.com

'''
Step 1 : intall all packages
'''

- **pip install beautifulsoup4** (Beautiful Soup for scraping and parsing data from the Web)
- **pip install lxml** (A method that helps python to parse html files/ tags and elements,
                    the best parser for beautifulsoup is lxml, it helps well in parsing bad html code,
                    the other parser for beautifulsoup is html5lib )
'''
step 2 : Fetch HTML contents of given url as string
'''                    

as here we donot use a website but a html file already in our system so we just fetch it by with open statement instead of :
url = input("url please : ") #"https://sundas-portfolio.herokuapp.com/"
r = requests.get(url) # get request for desired url
htmlContent = r.content
also that this file is in same directory as in which we have our python file so we just use "home.html" :
