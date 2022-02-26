
#cPanel settings for git hub repo deployment
- sign in to cPanel add files to file manager > public_html .. 
     follow tutorial https://tinyurl.com/nhapbw9k or https://tinyurl.com/2p86jdsz
     
- in git version control create a repositories or clone a url from github : tutotial here https://tinyurl.com/5fyuu38r
- 
- in side your project files create a file named to .cpanel.yml 

and add the following:

---<br>
deployment:<br>
  tasks:<br>
    - export DEPLOYPATH=/home/headw086/public_html/<br>
    - /bin/cp * $DEPLOYPATH<br>
    
    here a guide documentation : https://documentation.cpanel.net/display/CKB/Guide+to+Git+-+Deployment
    
 - To deploy on git version control Update from Remote then >>>Deploy HEAD Commit
