# _Terraform Module: terraform-module-aws-elasticache-cluster_


## _General_

_This module can be used to deploy a_ _**Elasticache Memcached Cluster** on AWS Cloud Provider......_


---

## _Prerequisites_

_This module needs **Terraform 0.12.20** or newer._
_You can download the latest Terraform version from_ [_here_](https://www.terraform.io/downloads.html).



---

## _Features Branches_

_Below we are able to check the resources that are being created as part of this module call:_

- _**Elasticache Memcached Cluster**_


---

## _Usage_

## _Using this repo_

_To use this module, add the following call to your code:_

```tf
module "elasticache_cluster" {
  source = "git::https://github.com/nitinda/terraform-module-aws-elasticache-cluster.git?ref=terraform-12/memcached"

  # Pass in relevant inputs required for this module here
  # e.g. vpc_id = "${data.terraform_remote_state.networking_shared_services.vpc_id}"

}
```


---

## _Inputs_

_The variables required in order for the module to be successfully called from the deployment repository are the following:_



---


## _Outputs_

### _General_

_This module has the following outputs:_

- _**cache\_nodes**_
- _**configuration\_endpoint**_
- _**cluster\_address**_



### _Usage_

_In order for the variables to be accessed at module level please use the syntax below:_

```tf
module.<module_name>.<output_variable_name>
```


_The output variable is able to be accessed through terraform state file using the syntax below:_

```tf
"${data.terraform_remote_state.<layer_name>.<output_variable_name>}"
```

---


## _Authors_

_Module maintained by Module maintained by the -_ **_Nitin Das_**