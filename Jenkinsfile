Groovy
pipeline {
 agent any
 stages {
 stage('Clone Repository') {
 steps {
 git url: 'https://github.com/Wajahat981/jenkins-websiteci.git'
 }
 }
 stage('Build Website') {
 steps {
 sh './hello.sh'
 }
 }
 stage('HTML Validation') {
 steps {
 echo 'Running HTML Validation...'
 sh 'tidy -q -e index.html || echo "HTML issues detected!"
