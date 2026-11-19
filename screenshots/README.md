# Screenshot Evidence Index

This index maps the **15 original screenshots** supplied for the AWS VPC Flow Logs monitoring project to the sections of the main [README](../README.md). Images are sanitized for sharing: AWS account identifiers and public IP addresses should not be visible in the uploaded copies.

> **Upload status:** The screenshot files are supplied in the GitHub-ready project ZIP, but they have **not been committed to this repository yet**. Upload the matching files into this `screenshots/` folder and their images in the main README will render automatically.

| # | Filename | What it verifies |
|---|---|---|
| 01 | `01-vpc-topology.png` | Both VPCs available; VPC 2 subnet and route table |
| 02 | `02-ec2-launch-network.png` | VPC 1 EC2 launch network and security group selections |
| 03 | `03-running-ec2-instances.png` | Two running EC2 instances and passed status checks |
| 04 | `04-cloudwatch-log-group.png` | CloudWatch log group creation confirmation |
| 05 | `05-vpc-flow-logs-trust-policy.png` | IAM trust policy allowing VPC Flow Logs to assume the role |
| 06 | `06-active-vpc-flow-log.png` | Active flow log on VPC 1, CloudWatch destination and role |
| 07 | `07-private-ping-initial-failure.png` | Private-IP ICMP failure before peering and routing |
| 08 | `08-public-ping-success.png` | Successful public-IP ICMP replies |
| 09 | `09-peering-request.png` | VPC 1 to VPC 2 peering request, pending acceptance |
| 10 | `10-vpc1-peering-route.png` | Active VPC 1 route to VPC 2 through `pcx-` |
| 11 | `11-vpc2-peering-route.png` | Active reciprocal VPC 2 route to VPC 1 |
| 12 | `12-cloudwatch-accept-reject-events.png` | CloudWatch traffic records with ACCEPT/REJECT actions |
| 13 | `13-expanded-rejected-flow-record.png` | Expanded REJECT flow-log entry |
| 14 | `14-log-analytics-interface.png` | CloudWatch revised Log Analytics UI |
| 15 | `15-top-10-byte-transfers.png` | Logs Insights Top 10 by transferred bytes |

**Evidence integrity:** The screenshot showing the peering request captures a **pending** state. The route-table images show active reciprocal routes later in the process. The successful private-IP ping was recorded in the project notes but is not shown in this image set.

**Safety:** Never upload access keys, authentication tokens, passwords, private keys, or unredacted account information. Temporary broad SSH/ICMP access should be removed or restricted after the lab.
