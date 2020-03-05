pipeline{
	agent any
	stages{
		stage('Clone'){
			steps{
			dir("D:\\CloneDIR\\") {
    			git branch: 'master', credentialsId: '3d5cdb37-6e90-465b-9b1d-527ae99e152d', url: 'https://github.com/Ritik180/Phase1-WithoutUsingBranches-.git'
				}
				echo "$BUILD_ID"
			}
		}
			stage('Bootstrap target configuration'){
				steps{
					configFileProvider([configFile(fileId: 'DEV.properties', variable: 'DEV')]) {
    						mvn clean deploy -DmuleDeploy -Dmaven.properties=$DEV
					}
				}
			}
		stage('Set Version'){
				steps{
					echo "stage done"
				}
			}
		stage('Munit Test'){
				steps{
					echo "stage done"
				}
			}
		stage('Maven Build and Deploy to Exchange'){
				steps{
					echo "stage done"
				}
			}
		}
	}

