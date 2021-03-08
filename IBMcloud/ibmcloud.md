Deploying MSSQL Server as a container on OCP follows the very good tutorial of 
*`https://github.com/johwes/sqlworkshops-sqlonopenshift`*

I had to change the deployment yaml file which you can also find in this folder.

Prerequisites: Download and install the oc client from your OCP cluster
Login to your OCP cluster using the CLI
Run following commands:

Step1: `./step1_create_project.sh` [show code](step1_create_project.sh)
 
Step2: `./step2_create_secret.sh`[show code](step2_create_secret.sh)

 
Step3: `./step3_storage.sh`[show code](step3_storage.sh)

 
Step4: `./step4_deploy_sql.sh`[show code](step4_deploy_sql.sh)

 
Step5: `./step5_get_errorlog.sh` [show code](step5_get_errorlog.sh)

