#!groovy

@Library('pipelib')
import org.veupathdb.lib.Builder

node('centos8') {

sh "env"

def builder = new Builder(this)
checkout scm
#builder.gitClone(['https://github.com/VEuPathDB/test_service.git': env.BRANCH_NAME])
builder.buildContainers([[name: 'test_service', path: '.']])

}
