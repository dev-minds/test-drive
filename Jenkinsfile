#!/usr/bin/env groovy
/**
  ***** MatchesFashion Devops ToolChain *****
  AIM: Automate simple and repetitive tasks 
  Owner: MAF Devops Team 
  Documentation: https://
  Status: Continouse Improvement 
https://groovy-lang.org/semantics.html
*/


def seperator60 = '\u2739' * 60
def seperator20 = '\u2739' * 20
def seperator30 = '\u2739' * 30

node() {
    stage('fetch repo') {
        echo "${seperator60}\n${seperator20} Checking out Source Repo \n${seperator60}"
        deleteDir()
        checkout scm
    }

    stage('Testing Job') {
        echo "${seperator60}\n${seperator20} Stage one job \n${seperator60}"
        sh """
            echo "Drive this process"
            bash test-script.sh 
        """
    }
}