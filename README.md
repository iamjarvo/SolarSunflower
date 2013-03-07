Solar Sunflower: A #TechCamp and Code for Philly Project
========================================================

The Solar Sunflower is an educational tool used for wireless monitoring of green stormwater infrastructure. Environmental data is collected by analog sensors (soil moisture, temperature, light) embedded in the green stormwater infrastructure system (e.g., a rain garden). Data is sent to the Web and can be mined by students or citizens and analyzed via an online interface. The data provides important information about system performance, plant health and maintenance needs.

To initialize:
`rake db:creat`
`rake db:migrate`
`rake db:seed`

login with user@example.com/changeme

To post soil moisture data to the database:

`curl -v -H "Content-Type: application/json" -X POST -d '{"type":"soilmoisture", "data":{"deptha":1,"depthb":1.2,"depthc":1.9}} ' 'http://localhost:3000/dc/'`
