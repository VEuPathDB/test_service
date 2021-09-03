#!groovy

@Library('pipelib@slack-notify')
import org.veupathdb.lib.Builder

node('centos8') {

sh "env"

def builder = new Builder(this)

builder.gitClone()
builder.buildContainers([[name: 'test_service']])

}
