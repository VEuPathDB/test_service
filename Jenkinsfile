#!groovy

@Library('pipelib@scm-info')
import org.veupathdb.lib.Project

node('centos8') {

  sh "env"

  Project.build(this) {

    component {

      docker 'test_service'
    }
  }
}
