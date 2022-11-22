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

![1](https://user-images.githubusercontent.com/33677647/203423729-7d9ff19d-b682-429e-ace1-a18ef81173de.JPG)

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

### Get all html h5 tags :

![1](https://user-images.githubusercontent.com/33677647/203420853-c6bd001d-a69f-4ee9-a71c-baf364f9d6a9.JPG)
![2](https://user-images.githubusercontent.com/33677647/203420864-fb8b3540-72da-4c36-b3c7-b7424c2bb4c7.JPG)

as all the courses names in our html are in h5, and the above script is giving the names of the courses with the whole tag, so lets use a for loop to fetch them, with out tags :

![2](https://user-images.githubusercontent.com/33677647/203423779-ae421169-6d4d-4aa1-abe2-cdca68b14c49.JPG)
![3](https://user-images.githubusercontent.com/33677647/203423796-f5900d7c-a2f1-427b-9282-69135fe7ebcf.JPG)

### Get name of all courses + their related course prices :

as all divs of all the courses have same class = 'card'.

![1](https://user-images.githubusercontent.com/33677647/203426319-8a6eaebe-16c2-49cd-a5fa-a3a0a2951efc.JPG)
![4](https://user-images.githubusercontent.com/33677647/203426458-ae0b5950-a982-46af-8aaf-2ae157777c7e.JPG)
![1](https://user-images.githubusercontent.com/33677647/203426940-038c6352-2175-473a-886e-25763c85d8d4.JPG)

As we see that in our all divs, it is h5 that have the names of all courses, it means we only need h5 in div.
so we use h5 tags as attributes ".h5" and got all h5 tags :

![1](https://user-images.githubusercontent.com/33677647/203427269-e38ab233-f7aa-4e46-89dd-d5370fbc5165.JPG)

as all the prices are also in anchor tags, so to fetch course name and price all together we do like :

![a](https://user-images.githubusercontent.com/33677647/203428525-2946ae5e-800c-4ee1-9ed0-d7666fae5b8a.JPG)
![b](https://user-images.githubusercontent.com/33677647/203428534-4a3337c5-6689-4887-8c93-e03415054e16.JPG)












