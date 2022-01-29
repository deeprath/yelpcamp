# yelpcamp
This repository contains a Simple camping ground Website where you can post, comment, get information about experiences, price.<br>
This Website is Developed using Nodejs,Bootsrap and MongoDB.<br>
This is a Study Project.<br>
You can Contribute, Comment and give Suggestions for the betterment of the Project.<br>
Thank You !!!<br>
Here is a working copy of Website: https://agile-reaches-28406.herokuapp.com/ <br>
<h1>Steps to start Working</h1>
<ol>
  <li><h3>Setup Node on your Machine</h3>
    <h4>Installing Node and NPM</h4>
    <code>sudo apt-get install nodejs</code><br>
    <code>sudo apt-get install npm</code>
  </li>
  <li><h3>Setup MongoDB</h3>
    <p>Totally optional if you don't want any database but it won't hurt to have some content in your mind to style better.</p>
    <h4>if mongo in not installed then type this command</h4>
    <code>sudo apt-get install mongodb</code><br>
    <ul>
      <li>Make a folder with name <b>data</b> in your home directory.<br>
        <code>mkdir data</code>
      </li>
      <li>Then create a file with name <b>mongod</b> in your home directory.<br>
      <code>touch mongod</code><br>
      <code>sudo chmod +777 mongod</code>
      </li>
      <li>finally open up file with gedit type following code<br>
        <code>mongod --dbpath=data --nojournal</code>
        <h4>OR type in terminal</h4>
        <code>echo "mongod --dbpath=data --nojournal">mongod</code>
      </li>
    </ul> 
  </li>
  <h3>Creating account on cloudinary, mongodb atlas and mapbox.</h3>
  <h4>mogodb atlas is required if you want to host your database on cloud.</h4>
    <ul>
      <li>Create a .env file and store your access credentials/Tokens</li>
      <code>CLOUDINARY_CLOUD_NAME=put_your_cloud_name</code><br>
      <code>CLOUDINARY_KEY=put_your_key</code><br>
      <code>CLOUDINARY_SECRET=put_your_secret_key</code><br>
      <code>MAPBOX_TOKEN=put_your_token</code><br>
      <code>DB_URL=connect_to_mongodb_atlas_with_your_password-follow_the_mongodb_instructions.</code><br>
    </ul>
  <li><h3>Finally running the app locally or on cloud</h3>
  <ul>
    <li>Run the Mongo Configuration File you Created above</li>
    <code>./mongod</code>
  <li>navigate to the main folder where app.js is located and type</li>
      <code>node app.js</code>
    </ul>
    </li>
</ol>
<br><br>
<h4>==================================</h4>
<h3>If your mongod service is giving you some error</h3>
<p><pre>2019-11-04T16:25:39.537+0530 E STORAGE  [initandlisten] Failed to set up listener: SocketException: Address already in use
2022-01-28T16:25:39.537+0530 I CONTROL  [initandlisten] now exiting
2022-01-28T16:25:39.537+0530 I CONTROL  [initandlisten] shutting down with code:48
</pre></p>
<h4>try these commands</h4><br>
<code>mongo</code><br>
<code>use admin</code><br>
<code>db.shutdowmServer()</code><br>
<code>db.shutdowmServer()</code><br>
this error is commonly due to some other service running on the port which mongo service listen is preoccupied by some other service

