# CourseProject

Please fork this repository and paste the github link of your fork on Microsoft CMT. Detailed instructions are on Coursera under Week 1: Course Project Overview/Week 9 Activities.

Author - Sean Lai
CS410

Improving the Educational Web System. 
This project is to improve the functionality of to save next slides in memory so users do not need to load each new slide every click.
Please read the documentation and instruction below on how to use EducationalWeb.

Please take a look at Documentation.docx, for more detail on how to use the software and how the software is implemented.


# Documentation/Instructions

The following instructions have been tested with Python2.7 on Linux and MacOS

1. You should have ElasticSearch installed and running -- https://www.elastic.co/guide/en/elasticsearch/reference/current/targz.html

2. Create the index in ElasticSearch by running `python create_es_index.py` from `EducationalWeb/`

3. Download tfidf_outputs.zip from here -- https://drive.google.com/file/d/19ia7CqaHnW3KKxASbnfs2clqRIgdTFiw/view?usp=sharing
   
   Unzip the file and place the folder under `EducationalWeb/static`

4. Download cs410.zip from here -- https://drive.google.com/file/d/1Xiw9oSavOOeJsy_SIiIxPf4aqsuyuuh6/view?usp=sharing
   
   Unzip the file and place the folder under `EducationalWeb/pdf.js/static/slides/`
   
5. From `EducationalWeb/pdf.js/build/generic/web` , run the following command: `gulp server`

6. On line 38 on `EducationalWeb/app.py`, edit the value here to an Integer for "number of slides to buffer at a time".
    
   I have set the default to "5", so you can also leave it as is.

7. In another terminal window, run `python app.py` from `EducationalWeb/`

8. The site should be available at http://localhost:8096/




