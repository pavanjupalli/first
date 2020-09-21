pipeline {
environment {

    PATH = "C:\\Windows\\System32"
}


agent any
stages {
stage('build') {
   steps {
withMaven(maven: 'maven-3') {
    echo 'i am at compile'

    sh 'mvn  compile'
}}}
stage('testing') {
   steps {
withMaven(maven : 'apache-maven-3.6.3') {
bat'mvn test'
}}}
stage('packaging') {
   steps {
withMaven(maven : 'apache-maven-3.6.3') {
bat'mvn package'
}}}
}}
