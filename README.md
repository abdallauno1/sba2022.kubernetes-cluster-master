# SBA Kubernetes Cluster
* **Objective** - Create a CI/CD Pipeline that builds an image from github and deploys it to a kubernetes cluster
* **Purpose** - To demonstrate container orchestration skillset



##  Software Used in This Project
*  Git CLI
*  Docker
*  minikube
*  kubectl
*  Python
 * Flask
 * Jenkins

## Instructions
* Fork and clone this project locally.
* Create a respective `requirements.txt` to download any `pip` dependencies for this python project.
  * Ensure you `push` the newly created file: `requirements.txt`
* Create a `Dockerfile` to  build the image.  Push it to github
* Build the image
* Push image to one of your repos on  [Dockerhub](https://hub.docker.com/).
* Create a `kubernetes.yml` which will pull the aforementioned Dockerhub image and create 3 running copies of it.
* Use the `kubernetes.yml` to launch your application.  Push this file to your github repo as well.  If possible have jenkins start the app by this method.
* Write and run a script to determine the state of your kubernetes cluster including the information about the services, pods, nodes, ip addresses, etc.
  * upload script to github `kubernetes-cluster-information.sh`
  * run script and  redirect the output of the `kuberenetes-cluster-information.sh` to `kuberenetes-cluster-information-output`
  * push the script output to your github repo


### How to Download

#### Part 1 - Forking the Project
* To _fork_ the project, click the `Fork` button located at the top right of the project.


#### Part 2 - Navigating to _forked_ Repository
* Navigate to your github profile to find the _newly forked repository_.
* Copy the URL of the project to the clipboard.

#### Part 3 - Cloning _forked_ repository
* Clone the repository from **your account** into the directory where you keep projects e.g. ~/projects
  * clone the project by executing the following command:
    * `git clone https://github.com/MYUSERNAME/NAMEOFPROJECT`

## How to run this
* Upon executing `python web.py`, navigate to `localhost:8080` to view the webpage.

<img src="./VIEWME.gif">


## Grading SBA (1100 pts total)
	Points Breakdown

	* 150		 pushed a requirements.txt file to their repo
	* 150		 built the new image w/jenkins
	* 150		 pushed Dockerfile to repo
	* 150		 Pushed built image to dockerhub
	* 150		 deployed image to k8s cluster
	* 150	  screenshot showing their browser
	* 150		 script+output to show k8s cluster status, 400 points if output shows correct functioning(e.g. pods, nodes, deployments, etc... of app) output+script pushed to github
	* 50		 submitted pull request with all their changes


## How to Submit

#### Submitting assignment
* from the browser, navigate to the _forked_ project from **your** github account.
* click the `Pull Requests` tab.
* select `New Pull Request`
