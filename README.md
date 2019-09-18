# Tutorial Google Cloud Platform

Welcome to Google Cloud - Deep Dive Series
--------------------------------------------------------------------

1. GCP is responsible for security _(of)_ the cloud and Users are
responsible for security _(in)_ cloud

(A) Cloud IAM
-----------
- let you manage access control by defining <who> has 
  access for <which> resource
- principle of least priviledge : gain only the necessary access to 
  your resource
  
(B) WHO
-----------
1. Google Accounts (frankyeung1996@gmail.com)
  - can be a developer, admin, or any other actual
     user who interact with GCP
2. Service Account 
  - Application that you deploy (apps/scripts)
3. Google Groups (e.g. Ggroup1@googlegroups.com)
   - named collection of gmail ids
   - unique name and an email id
   - single point to apply an access policy to a 
     collection of users
   - GSuite Domain (Gmail, Google Drive)
   - Cloud Identity domain (IDaaS)  (hsbc.com, infosys.com)
   - Federated Users (single sign-on (SSO))
  
(C) Concepts related to Cloud IAM
-----------
1. Resource
  - anything that you create within GCP - VM instance, storage bucket
2. Permissions
  - determine what operations are allowed on a resource
  - they are represented in the form of <service>.<resource>.<verb>
      - compute.instances.delete
      - appengine.instances.list
      - pubsub.subscriptions.consume
3. Roles
