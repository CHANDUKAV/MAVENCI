#!/usr/bin/env groovy
pipeline {
agent any
stages {
  stage ('Compile Stage') {
    steps {
      withMaven(maven : 'maven_3_5_3') {
         sh 'mvn clean compile'
}
}
}
 stage ('Testing Stage') {
    steps {
      withMaven(maven : 'maven_3_5_3') {
         sh 'mvn test'
}
}
}
 stage ('Deployement Stage') {
    steps {
      withMaven(maven : 'maven_3_5_3') {
         sh 'mvn deploy'
}
}
}
}
}
