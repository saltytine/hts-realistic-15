# much bigger writeup  
this one took a long time  

The blurb blurbs at us  
![image](https://github.com/user-attachments/assets/1c26a44c-ed06-47fd-83af-aa344d93a43a)  

This is the main page  
![image](https://github.com/user-attachments/assets/5b3e160d-24f8-4450-b01c-e47517c18716)  
and there are a few other main pages:  
products:  
![image](https://github.com/user-attachments/assets/1b97c389-db8c-4eec-814c-3777eb720abf)  
questions:  
![image](https://github.com/user-attachments/assets/b79f7aec-9f19-473b-9abf-8aef65164f47)  
imprint:  
![image](https://github.com/user-attachments/assets/05a7dc0c-29e9-4dda-bc5c-17a8f1b4fae7)  
and jobs:  
![image](https://github.com/user-attachments/assets/4618af46-fb2c-478c-8d7d-36049b95cc8f)  
back to questions, if i send a message, the site shows this:  
![image](https://github.com/user-attachments/assets/c7ed61ed-1b15-4d1a-9fcb-1f214f1e2cf2)  
their checkmark looks awful, its in an images folder, which is nice to know they have  
![image](https://github.com/user-attachments/assets/e32ddac9-f492-4426-89e0-485e00c59f6e)  
burpsuite shows all the forms that we left unfilled:  
![image](https://github.com/user-attachments/assets/454f402b-97b6-4b41-b52e-8944f310c4a8)  
out of curiosity, i visited the image folder and it has a bunch of iamges, unsurprisingly  
![image](https://github.com/user-attachments/assets/c9cf2fdd-9687-4c90-a722-da4dc514e03b)  
nothing special  
not many of the other pages have anything of interest other than jobs, which has a place to submit you application  
![image](https://github.com/user-attachments/assets/3fc507c7-732e-4286-bacf-64ed2363bea9)  
it looks almost identical to the other submission page  
![image](https://github.com/user-attachments/assets/2ee38c71-1e2f-479b-95f0-db57752deb0b)  
submitting shows the same in burpsuite and the same on the page  
![image](https://github.com/user-attachments/assets/96f365be-cd99-4b6f-8f31-8ca95ef986b9)  
but this is different because the page pulls this image from a backups folder  
![image](https://github.com/user-attachments/assets/96e2afd8-03f2-46e9-a2f1-a19a9aed84df)  
you can visit the backups folder to find the images folder and a backup.zip file  
![image](https://github.com/user-attachments/assets/44f29adf-6d41-4a75-923c-74507d76f322)  
i downloaded the zip file, but its all password protected  
so i used pkcrack  
using windows i can see all of the files in the zip, i just cant open them  
![image](https://github.com/user-attachments/assets/98f8f394-b08b-4bc4-ae12-e53461b0e48e)  
these in a folder called internal_messages  
![image](https://github.com/user-attachments/assets/582824b1-e2b0-4600-a7f3-afd943850920)  
and these in a misc folder  
in order to use pkcrack we need a file thats identical and zipped, but missing a password  
so we need to find one of the files in the folder, on the site  
its just the main page  
i compaired the sizes of the two and they seem to be exactly the same, so the hope is that the folder is exactly the same  
