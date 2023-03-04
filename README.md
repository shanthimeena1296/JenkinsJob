# JenkinsJob

echo "# JenkinsJob" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin git@github.com:shanthimeena1296/JenkinsJob.git
git push -u origin main

docker run -p 8080:8080 -v jenkins_home:/var/jenkins_home jenkins/jenkins:lts-jdk11

run the above command for running the docker myjenkinsjob
