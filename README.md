This is just a small project with Continous deployment using a bash script after the contents are pushed via git to the remote repo. 

WORKING:
============
The changes are made to the contents folder. Once a change is done and pushed to the remote repo. Either set a set cron (POll SCM) which polls continuously for any changes in the repo or use GitHub hook trigger for GITScm polling to create the webhook. It will inturn trigger the ansible-playbook via the pipeline code in the Jenkinsfile within the SCM. The Docker image build will only happen when a change is occured in the repository no matter how many times you manually run the playbook.
