# classCentralClone
This was a challenge for an interview. The idea was to use the software HTTrack to copy a site and then use the Google Translate API to translate the html files to hindi with this last part being done by changing the html itself, so you should have the hindi hardcoded into the html file. So what I've done is use the library translate in python that has been created by reverse engineering the Google Translate API. So first you have to open the translateTest.py and then you will see how this is implemented. First I import everything that we are going to use, then I created a function that just takes some string and translate it to hindi using this library and it returns a string. Then I built a recursive function to go through the entire directory and any directory inside of the first one and creates an array with the directory direction to every .html file that is on the directory. Then I use a library called HTMLParser, that do just that, it reads the htrml files that we saved before and go through it line by line, or actually tag by tag. In every tag it takes what is inside and translate it to hindi using the function that I created at the start of this code. Then creates a temporary copy of the html but in hindi and finally there is a function that replace the original html file for the copy in hindi. 

As you can see it works, I created a copy of the home page of https://www.classcentral.com/ and the translation works. There are a lot of bugs to fix, for example for now we are ignoring a lot of tags like anchor tags that may have some text that we want to translate so it's not done. This repository is public so anyone can take this code and do what they please with it, it was a fun project and there is still a lot to do. But when finished we will be able to use it to translate any kind of file, not just html files, to any lenguage. So that is a really amazing. As it is built now, the code only should take html files, so bear that in mind. 

I hope you enjoy this project as did I. 

You can access the site here: 

https://clonedemo-ariel-oliveira.netlify.app/

