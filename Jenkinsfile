pipeline {
agent any
stages {
stage('Information') {
steps {
powershell '''
$ErrorActionPreference = 'Stop'
Write-Host "Machine : $env:COMPUTERNAME"
Write-Host "Compte :
$([System.Security.Principal.WindowsIdentity]::GetCurrent().Name)"
Write-Host "Job : $env:JOB_NAME"
Write-Host "Build : $env:BUILD_NUMBER"
Write-Host "Workspace : $env:WORKSPACE"
'''
}
}
}
}
