# A better PHP redirect_to function

### Are you looking to avoid the "headers already sent" error?   
### This function may be the answer you seek.  
  
First the function checks if headers were sent,  
Next it verifies that a destination was given,  
Next it checks if the page is numeric (404 etc), 
Now if headers were not sent - header(Location: ) runs,  
If the headers were sent then the function tries with Javascript,  
If Javascript is turned off then it becomes an HTML refresh.  
