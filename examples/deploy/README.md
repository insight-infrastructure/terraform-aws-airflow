# How to create a basic cluster and deploy some DAGs


## Usage

Before running the commands above make sure to create a file named `terraform.tfvars` 

To run this example you need to execute:

```
$ terraform init
$ terraform plan
$ terraform apply
```

Note that this example may create resources which cost money. Run `terraform destroy` when you don't need these resources.

**WARNING - Database passwords and Fernet Key are hardcoded in the sample configuration: do not use these in production**


<!-- BEGINNING OF PRE-COMMIT-TERRAFORM DOCS HOOK -->
## Outputs

| Name | Description |
|------|-------------|
| database\_endpoint | Endpoint to connect to RDS metadata DB |
| database\_username | Username to connect to RDS metadata DB |
| this\_cluster\_security\_group\_id | The ID of the security group |
| this\_database\_security\_group\_id | The ID of the security group |
| webserver\_admin\_url | Public DNS for the Airflow Webserver instance |
| webserver\_public\_ip | Public IP address for the Airflow Webserver instance |

<!-- END OF PRE-COMMIT-TERRAFORM DOCS HOOK -->