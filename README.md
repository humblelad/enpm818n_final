# enpm818n_final

Steps:
phasenat.yaml is the acutal fully completed cft for Phase 1 . (phase1.yaml is also same but it has public subnet as well as ssh setup)
I recommend deploying phasenat.yaml and then using aws ui > eks client instance / docker instance > connect> connect via ssm for better security. 

Instructions for Phase 2:
deploy forphase2.yaml as stack . I have commented out docker deployment piece from phase 1 as you only need eks deployment. You have to do the application setup via help instead of k8 in a new namespace . 

Phase 3,4 can also work simaltaneously via first deploying forphase2.yaml or phasenat.yaml ( if you use this the application would run through docker as well)  . 

Note you can only ssm to the instance and you may have to do sudo su and only as root user run commands. First verify if kubectl version works. 
