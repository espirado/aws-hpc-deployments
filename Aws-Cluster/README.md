# Icipe-AWS-cluster-template
AWS ParallelCluster is an AWS supported open source cluster management tool that helps you to deploy and manage High Performance Computing (HPC) clusters in the AWS Cloud. Built on the open source CfnCluster project, AWS ParallelCluster enables you to quickly build an HPC compute environment in AWS. 



# Template Usage 
The main aim of the template is to assist icipe team to provision parrallel clusters fast and efficient without having to know the underlying technical details.

#### template performs the following 

- Install and configure ParallelCluster on your AWS Cloud9 IDE.
- Create your first cluster.
- Submit your job and check what is happening in the background.
- Delete the cluster.



### Underlying infrastucture 

![Work Design](https://github.com/espirado/Icipe-computing-Research/blob/main/Images/pc-architecture.png)


# USER GUIDE
 - run pcluster create-cluster --cluster-name $cluster-name --cluster-configuration configuration.yaml

 # view clusters created

-  pcluster list-clusters

# ssh into cluster 

- pcluster ssh --cluster-name $cluster-name -i $ssh-pair-key

# submit your job using slurm
- sbatch $job-name 


# Delete cluster 

pcluster delete-cluster --cluster-name $cluster-name
