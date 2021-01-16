Debugging process for configuring our IAM users for our cluster:

Link used for solution: https://docs.aws.amazon.com/eks/latest/userguide/add-user-role.html

- https://docs.aws.amazon.com/eks/latest/userguide/add-user-role.html

- I basically copied and pasted this doc and added a map users section under with the name of our eks-cluster-admin + the arn 

- I took the arn of our original role arn in  aws-auth configmap file and just used that

- when running it sucessfully configured but still cant make any eksctl api calls, only kubectl works 

- basically just delete the bottom section of the default configmap and add the users to the mapuser section + add configmap kind at the top 
