# jsonkmean

this is the javascript object parsed that i exported from MongoDB to use for AWS data entry


===================mongo with biomean ===============================

My biomean application stringify local jsonarray on each chart which can not be used for mongo tools
I used mongoexport to generate json objects which then I could import it on EC2 instance

mongoexport --collection BMPDocs --db biomeandb --out=bmp.json
2022-01-05T13:27:41.986-0500	connected to: mongodb://localhost/
2022-01-05T13:27:41.993-0500	exported 11 records

Used GitHub to export kmean into EC2

mongoimport —host localhost —db biomeqndb —collection BMPDocs —type json —file ./kmean.json
mongoimport —host localhost —db biomeqndb —collection BMPDocs —jsonArray —file ./kmean.json (did not work)
￼

for enforcing node app to run in background i used :

#npm install forever -g
#forever start server.js


https://github.com/foreversd/forever
