#!groovy

@Library('pipelib')
import org.veupathdb.lib.Builder

node('centos8') {

sh "env"

checkout scm

def builder = new Builder(this)
builder.buildContainers([[name: 'test_service']])

}
