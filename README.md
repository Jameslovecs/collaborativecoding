# collaborativecoding

* Technologies:
1. AngularJS
2. NodeJS
3. SocketIO
4. ACE editor API
5. Autho0
6. Redis
7. MongoDB
8. Docker
9. Flask
10. Nginx
11. RESTful API
12. JavaScript
13. Python




* How-To:
1. How to start Nginx server:
	sudo nginx -s signal
	
	signal:
		stop - fast shutdown
		quit - graceful shutdown
		reload - reloading the configuration file
		reopen - reopening the log files

2. Copy configuration files from 'sites-available' to 'sites-enabled':
	ln -s ../sites-available/example ./example

3. Change hosts file:
	cat /etc/hosts

4. Install nginx by homebrew
	brew install nginx

5. To run the program:
	a. Go to oj-client folder: run 'ng build -watch'
	b. Go to oj-server folder: run 'nodemon server.js'
	c. Go to redis-3.2.9 2/src/: run 'redis-server'

6. Installed node-rest-client:
	node i --save node-rest-client
	To make the oj-server as a client that can sent rest requests

7. Installed flask:
	sudo pip install --upgrade pip
	sudo pip install flask

8. To run flask server:
	python executor_server.py

9. docker:
	docker ps -a
	docker images
	stop all containers: docker stop $(docker ps -a -q)
	remove all containers: docker rm $(docker ps -a -q)
	build: sudo docker build . -t jylock/cs503_1703
	login: docker login
	push: docker push jylock/cs503_1703
	pull: docker pull jylock/cs503_1703
	delete all images: docker rmi $(docker images -a -q)

10. install docker so that python can communicate with docker, just like nodejs communicate with reddis
	sudo pip install docker

11. Need to have oj-client, oj-server, executor_server, redis, and nginx running simutaneously