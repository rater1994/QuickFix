# QuickFix 

<br>

<b>Command for mysql linux</b>

 ``service mysql status / restart / start``
 
 ``service apache2 restart / start / status``
   
    
<b> Add user to mysql database </b>

``CREATE USER 'usernameForServer'@'localhost' IDENTIFIED BY 'passwordForUser';``

``GRANT ALL PRIVILEGES ON * . * TO 'usernameForServer'@'localhost';``


<b>Add boostrap to angular</b>

 ``npm install bootstrap@3 --save``


  Add in angular.json ->  
  ``styles": ["node_modules/bootstrap/dist/css/bootstrap.min.css",``

  Add in style.css:  
   ``@import '~bootstrap/dist/css/bootstrap.min.css';``
   
  
<b> Git remove from cache files</b>

``git rm --cached nameOfFile``

<b> Android studio - set kvm "acces denied" </b>

``sudo setfacl -m u:user:rwx /dev/kvm``

<b>Angular reload page watch memory size</b>

``sudo sysctl fs.inotify.max_user_watches=524288``

``sudo sysctl -p``

> If you like to make your limit permanent, use:

``echo fs.inotify.max_user_watches=524288 | sudo tee -a /etc/sysctl.conf
  sudo sysctl -p``


<b> Add fontawesome angular </b>

``npm install --save font-awesome``

 Add in angular.json 
 
 ``"../node_modules/font-awesome/css/font-awesome.css" or "node_modules/font-awesome/css/font-awesome.css"``



<b> Maven maping doesn't show in terminal </b>

``version:<version>2.1.0.RELEASE</version> change to: 2.0.6 <---``


<b> Error creating bean with name 'entityManagerFactory'</b>

```` 
<dependency>
          <groupId>javax.xml.bind</groupId>
          <artifactId>jaxb-api</artifactId>
          <version>2.3.0</version>
  </dependency>
````


<b>Dpk debian pubkey expired in 2019.01.01 </b>

``	wget -qO - https://raw.githubusercontent.com/yarnpkg/releases/gh-pages/debian/pubkey.gpg | sudo apt-key add -
``


<b> Post method in PostMan  Invalid cors error </b>

``Add in Headers: Origin      http://localhost:8080``