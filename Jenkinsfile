// This shows a simple build wrapper example, using the AnsiColor plugin.
	
	pipeline { 
		agent any
		triggers { pollSCM('* * * * *') }
		stages {
			
			
			stage('Desplegar Pruebas') { 
				steps { 
					git branch: 'master',url: 'https://github.com/mauro2357/KitBasicoAutomApp-Ops.git'
					bat 'xcopy "config" "KitBasicoAutomApp/build/libs"'
					bat "deploy.bat"
				}
			}
			
		}
		
	}

