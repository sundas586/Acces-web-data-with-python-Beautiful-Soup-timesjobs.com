# Acces-web-data-with-python-Beautiful-Soup-timesjobs.com

'''<br/>
Step 1 : intall all packages<br/>
'''<br/>

- **pip install beautifulsoup4** (Beautiful Soup for scraping and parsing data from the Web)<br/>
- **pip install lxml** (A method that helps python to parse html files/ tags and elements,
                    the best parser for beautifulsoup is lxml, it helps well in parsing bad html code,
                    the other parser for beautifulsoup is html5lib )<br/>

'''<br/>
step 2 : Fetch HTML contents of given url as string<br/>
'''<br/>         

as here we donot use a website but a html file already in our system so we just fetch it by with open statement instead of :<br/>
r = requests.get(url) # get request for desired url<br/>
htmlContent = r.content<br/>
also that this file is in same directory as in which we have our python file so we just use "home.html" :<br/>

![1](https://user-images.githubusercontent.com/33677647/203418122-a46cf0c7-f888-45a2-a4f8-20af3051da4a.JPG)

'''<br/>
step 3 : Parse the HTML string<br/>
'''<br/>

![2](https://user-images.githubusercontent.com/33677647/203418583-18d630fa-304c-4f47-bcf3-8d709de4e4fe.JPG)

'''<br/>
step 4 : HTML tree traversal<br/>
'''<br/>

### get all html h5 tags :

![1](https://user-images.githubusercontent.com/33677647/203420853-c6bd001d-a69f-4ee9-a71c-baf364f9d6a9.JPG)
![2](https://user-images.githubusercontent.com/33677647/203420864-fb8b3540-72da-4c36-b3c7-b7424c2bb4c7.JPG)





