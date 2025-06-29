---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "octopusdeploy_git_credentials Data Source - terraform-provider-octopusdeploy"
subcategory: ""
description: |-
  Use this data source to retrieve information about Git credentials in Octopus Deploy.
---

# octopusdeploy_git_credentials (Data Source)

Use this data source to retrieve information about Git credentials in Octopus Deploy.



<!-- schema generated by tfplugindocs -->
## Schema

### Optional

- `name` (String) The name of the Git Credential to filter by.
- `skip` (Number) The number of records to skip.
- `space_id` (String) The space ID associated with this Git Credential.
- `take` (Number) The number of records to take.

### Read-Only

- `git_credentials` (Attributes List) Provides information about existing GitCredentials. (see [below for nested schema](#nestedatt--git_credentials))
- `id` (String) The unique ID for this resource.

<a id="nestedatt--git_credentials"></a>
### Nested Schema for `git_credentials`

Read-Only:

- `description` (String) The description of this Git Credential.
- `id` (String) The unique ID for this resource.
- `name` (String) The name of this Git Credential.
- `repository_restrictions` (Attributes) Sets the repository restrictions associated with the Git credential. (see [below for nested schema](#nestedatt--git_credentials--repository_restrictions))
- `space_id` (String) The space ID associated with this Git Credential.
- `type` (String) The Git credential authentication type.
- `username` (String) The username for the Git credential.

<a id="nestedatt--git_credentials--repository_restrictions"></a>
### Nested Schema for `git_credentials.repository_restrictions`

Read-Only:

- `allowed_repositories` (Set of String) Set of allowed repository URL's.
- `enabled` (Boolean) Whether repository restrictions are enabled.


