pipeline {



agent any
stages {
stage('build') {
   steps {
withMaven(maven : 'apache-maven-3.6.3') {
bat'mvn clean compile'
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
