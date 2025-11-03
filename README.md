##  VPC Traffic flow and security ##
## Overview ##
In this project i have created **Route tables** , **Security groups** and **Network ACL (Access control list)**.
## Architecture diagram ##

<pre>
+----------------------------------+
|        VPC (10.0.0.0/16)         |
|                                  |
|   +--------------------------+   |
|   |     Internet Gateway     |   |
|   +------------+-------------+   |
|                |                 |
|   +--------------------------+   |
|   |      Route Table         |   |
|   |  0.0.0.0/0 → IGW         |   |
|   +------------+-------------+   |
|                |                 |
|   +--------------------------+   |
|   |      Public Subnet       |   |
|   |      (10.0.0.0/24)       |   |
|   |   +------------------+   |   |
|   |   |  Security Group  |   |   |
|   |   +------------------+   |   |
|   +--------------------------+   |
|          Network ACL             |
+----------------------------------+
</pre>

## Steps followed ##
1. Created a **Route table** and attached to the **public subnet** by editing subnet association.
2. Next Created a **security group** and added inbound  rule.
3. Created **Network ACL** And created inbound and outbound rules.and then attached to subnet.


## Screenshots ##
<img width="3394" height="1088" alt="Image 11-3-25 at 12 44 AM (1)" src="https://github.com/user-attachments/assets/87303d26-4bff-4814-8ddc-9221843dc5b9" />

<img width="2936" height="976" alt="Image 11-3-25 at 12 46 AM" src="https://github.com/user-attachments/assets/14a1bced-377e-4427-bba8-aebee88227a3" />

<img width="2904" height="988" alt="Image 11-3-25 at 12 47 AM" src="https://github.com/user-attachments/assets/f0be8e92-eb8a-44cb-a58d-3d471bf5ed60" />

<img width="2926" height="1052" alt="Image 11-3-25 at 12 46 AM 2" src="https://github.com/user-attachments/assets/48ffd1bf-706d-42db-8ec5-73b3447a6598" />

<img width="2912" height="1136" alt="Image 11-3-25 at 12 46 AM (1)" src="https://github.com/user-attachments/assets/700e8fad-fa9b-4ce5-aa21-6b82766cc233" />

<img width="976"  height="651" alt="Part2 architecture drawio" src="https://github.com/user-attachments/assets/a82ce65f-f29c-4325-9026-cd93aca0fe1a" />

## Key learnings ##
- Learned about route tables and how they are used to distribute or send the data to its desitination
- Acheived an idea on security groups and learned how to update inbound rules.
- Learned about Rule number 100.
- Learned about Network ACL And rules.

## Next steps ##
In the next project i will extend this seup and build Private subnet.




