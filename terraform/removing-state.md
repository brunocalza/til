When you want that an item it is no longer managed by Terraform, you can remove it from Terraform state.

I needed this because I manually deleted an instance of BigTable on GCP that was created using Terraform. There was a mismatch between Terraform state and the GCP resource.

From [docs](https://www.terraform.io/docs/commands/state/rm.html): the example below removes the `packet_device` resource named `worker`:

```$ terraform state rm 'packet_device.worker'```