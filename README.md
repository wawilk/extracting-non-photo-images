
# Demo Notebook

## How to get the non-photo images from a PDF document

The purpose of this notebook is to demonstrate how to save embedded images  
that are not photos but line drawings and tables to disk and give them  
a meaningful name to help with retrieval.  

These types of images are not identified as images when using pypdf but can be found using OpenCV.  
We will look at that approach.  

## How to construct image file names

Once we have an image identified we also need to name it in a way that so it can be easily retieved by front end apps. An example would be an Azure Open AI RAG app that returns answers to questions based on a document as contecxt. You may want to display the image if the answewr refernce the figure in the answer.

As one possible solution, we will explore using Azure Document Intelligence to OCR'd text from a List of Figures and a list of Tables contained in the document itself. We will then parse the text to come up with names that can easily be mapped back to references in the document.
