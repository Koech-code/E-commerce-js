## DANCO SOLUTIONS
1. Create folder structure
 1. create root folder as we
 2. add frontend and backend folder
 3. create src folder in frontend
 4. create index.html in src 
 5. run `npm init` in frontend folder
 6. install live-server by `npm install live-server`
 7. add start command as live-server --verbose
 8. run `npm start` to serve your app on default browser

2. Design website
 1. create a file named styles.cc
 2. link the styles file to index.html file
 3. create a div.grid-container
 4. create header, main and footer
 5. style the html, body using css
 6. style grid-container, header, main and footer

3. Create static home screen
 1. create a list of products
 2. add images
 3. style products

4. Render dynamic homepage
 1. create data.js
 2. export an array of products
 3. create screens/Homescreen.js
 4. export homescreen as an object with render() method
 5. implement render()
 6. import data.js
 7. return products mapped to list as ul
 8. create app.js
 9. link it to index.html as module
 10. set main id to main-container
 11. create router() function
 12. set main_container innerHtml to Homescreen.render()
 13. set load event of window to render() function

5. Build URL router
 1. create routes as route:screen object for home screen
 2. create utils.js
 3. export parseRequestURL()
 4. set URL as harsh address split by slash
 5. return resource, id and verb of URL
 6. update router()
 7. ser request as parseRequestURL()
 8. build parsedURL and compare with routes
 9. if route exist render it, else render Error404
 10. create screens/error.js and render error message