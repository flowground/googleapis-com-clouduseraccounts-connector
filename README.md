# ![LOGO](logo.png) Cloud User Accounts **flow**ground Connector

## Description

A generated **flow**ground connector for the Cloud User Accounts API (version vm_alpha).

Generated from: https://api.apis.guru/v2/specs/googleapis.com/clouduseraccounts/vm_alpha/swagger.json<br/>
Generated at: 2019-05-23T12:13:08+03:00

## API Description

Creates and manages users and groups for accessing Google Compute Engine virtual machines.

## Authorization

Supported authorization schemes:
- OAuth2
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Retrieves the list of groups contained within the specified project.

*Tags:* `groups`

#### Input Parameters
* `filter` - _optional_ - Sets a filter expression for filtering listed resources, in the form filter={expression}. Your {expression} must be in the format: field_name comparison_string literal_string.

The field_name is the name of the field you want to compare. Only atomic field types are supported (string, number, boolean). The comparison_string must be either eq (equals) or ne (not equals). The literal_string is the string value to filter to. The literal value must be valid for the type of field you are filtering by (string, number, boolean). For string fields, the literal value is interpreted as a regular expression using RE2 syntax. The literal value must match the entire field.

For example, to filter for instances that do not have a name of example-instance, you would use filter=name ne example-instance.

Compute Engine Beta API Only: If you use filtering in the Beta API, you can also filter on nested fields. For example, you could filter on instances that have set the scheduling.automaticRestart field to true. In particular, use filtering on nested fields to take advantage of instance labels to organize and filter results based on label values.

The Beta API also supports filtering on multiple expressions by providing each separate expression within parentheses. For example, (scheduling.automaticRestart eq true) (zone eq us-central1-f). Multiple expressions are treated as AND expressions, meaning that resources must match all expressions to pass the filters.
* `maxResults` - _optional_ - The maximum number of results per page that should be returned. If the number of available results is larger than maxResults, Compute Engine returns a nextPageToken that can be used to get the next page of results in subsequent list requests.
* `orderBy` - _optional_ - Sorts list results by a certain order. By default, results are returned in alphanumerical order based on the resource name.

You can also sort results in descending order based on the creation timestamp using orderBy="creationTimestamp desc". This sorts results based on the creationTimestamp field in reverse chronological order (newest result first). Use this to sort resources like operations so that the newest operation is returned first.

Currently, only sorting by name or creationTimestamp desc is supported.
* `pageToken` - _optional_ - Specifies a page token to use. Set pageToken to the nextPageToken returned by a previous list request to get the next page of results.
* `project` - _required_ - Project ID for this request.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters. Overrides userIp if both are provided.
* `userIp` - _optional_ - IP address of the site where the request originates. Use this if you want to enforce per-user limits.

### Creates a Group resource in the specified project using the data included in the request.

*Tags:* `groups`

#### Input Parameters
* `project` - _required_ - Project ID for this request.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters. Overrides userIp if both are provided.
* `userIp` - _optional_ - IP address of the site where the request originates. Use this if you want to enforce per-user limits.

### Deletes the specified Group resource.

*Tags:* `groups`

#### Input Parameters
* `groupName` - _required_ - Name of the Group resource to delete.
* `project` - _required_ - Project ID for this request.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters. Overrides userIp if both are provided.
* `userIp` - _optional_ - IP address of the site where the request originates. Use this if you want to enforce per-user limits.

### Returns the specified Group resource.

*Tags:* `groups`

#### Input Parameters
* `groupName` - _required_ - Name of the Group resource to return.
* `project` - _required_ - Project ID for this request.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters. Overrides userIp if both are provided.
* `userIp` - _optional_ - IP address of the site where the request originates. Use this if you want to enforce per-user limits.

### Adds users to the specified group.

*Tags:* `groups`

#### Input Parameters
* `groupName` - _required_ - Name of the group for this request.
* `project` - _required_ - Project ID for this request.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters. Overrides userIp if both are provided.
* `userIp` - _optional_ - IP address of the site where the request originates. Use this if you want to enforce per-user limits.

### Removes users from the specified group.

*Tags:* `groups`

#### Input Parameters
* `groupName` - _required_ - Name of the group for this request.
* `project` - _required_ - Project ID for this request.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters. Overrides userIp if both are provided.
* `userIp` - _optional_ - IP address of the site where the request originates. Use this if you want to enforce per-user limits.

### Gets the access control policy for a resource. May be empty if no such policy or resource exists.

*Tags:* `groups`

#### Input Parameters
* `project` - _required_ - Project ID for this request.
* `resource` - _required_ - Name of the resource for this request.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters. Overrides userIp if both are provided.
* `userIp` - _optional_ - IP address of the site where the request originates. Use this if you want to enforce per-user limits.

### Sets the access control policy on the specified resource. Replaces any existing policy.

*Tags:* `groups`

#### Input Parameters
* `project` - _required_ - Project ID for this request.
* `resource` - _required_ - Name of the resource for this request.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters. Overrides userIp if both are provided.
* `userIp` - _optional_ - IP address of the site where the request originates. Use this if you want to enforce per-user limits.

### Returns permissions that a caller has on the specified resource.

*Tags:* `groups`

#### Input Parameters
* `project` - _required_ - Project ID for this request.
* `resource` - _required_ - Name of the resource for this request.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters. Overrides userIp if both are provided.
* `userIp` - _optional_ - IP address of the site where the request originates. Use this if you want to enforce per-user limits.

### Retrieves the list of operation resources contained within the specified project.

*Tags:* `globalAccountsOperations`

#### Input Parameters
* `filter` - _optional_ - Sets a filter expression for filtering listed resources, in the form filter={expression}. Your {expression} must be in the format: field_name comparison_string literal_string.

The field_name is the name of the field you want to compare. Only atomic field types are supported (string, number, boolean). The comparison_string must be either eq (equals) or ne (not equals). The literal_string is the string value to filter to. The literal value must be valid for the type of field you are filtering by (string, number, boolean). For string fields, the literal value is interpreted as a regular expression using RE2 syntax. The literal value must match the entire field.

For example, to filter for instances that do not have a name of example-instance, you would use filter=name ne example-instance.

Compute Engine Beta API Only: If you use filtering in the Beta API, you can also filter on nested fields. For example, you could filter on instances that have set the scheduling.automaticRestart field to true. In particular, use filtering on nested fields to take advantage of instance labels to organize and filter results based on label values.

The Beta API also supports filtering on multiple expressions by providing each separate expression within parentheses. For example, (scheduling.automaticRestart eq true) (zone eq us-central1-f). Multiple expressions are treated as AND expressions, meaning that resources must match all expressions to pass the filters.
* `maxResults` - _optional_ - The maximum number of results per page that should be returned. If the number of available results is larger than maxResults, Compute Engine returns a nextPageToken that can be used to get the next page of results in subsequent list requests.
* `orderBy` - _optional_ - Sorts list results by a certain order. By default, results are returned in alphanumerical order based on the resource name.

You can also sort results in descending order based on the creation timestamp using orderBy="creationTimestamp desc". This sorts results based on the creationTimestamp field in reverse chronological order (newest result first). Use this to sort resources like operations so that the newest operation is returned first.

Currently, only sorting by name or creationTimestamp desc is supported.
* `pageToken` - _optional_ - Specifies a page token to use. Set pageToken to the nextPageToken returned by a previous list request to get the next page of results.
* `project` - _required_ - Project ID for this request.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters. Overrides userIp if both are provided.
* `userIp` - _optional_ - IP address of the site where the request originates. Use this if you want to enforce per-user limits.

### Deletes the specified operation resource.

*Tags:* `globalAccountsOperations`

#### Input Parameters
* `operation` - _required_ - Name of the Operations resource to delete.
* `project` - _required_ - Project ID for this request.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters. Overrides userIp if both are provided.
* `userIp` - _optional_ - IP address of the site where the request originates. Use this if you want to enforce per-user limits.

### Retrieves the specified operation resource.

*Tags:* `globalAccountsOperations`

#### Input Parameters
* `operation` - _required_ - Name of the Operations resource to return.
* `project` - _required_ - Project ID for this request.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters. Overrides userIp if both are provided.
* `userIp` - _optional_ - IP address of the site where the request originates. Use this if you want to enforce per-user limits.

### Retrieves a list of users contained within the specified project.

*Tags:* `users`

#### Input Parameters
* `filter` - _optional_ - Sets a filter expression for filtering listed resources, in the form filter={expression}. Your {expression} must be in the format: field_name comparison_string literal_string.

The field_name is the name of the field you want to compare. Only atomic field types are supported (string, number, boolean). The comparison_string must be either eq (equals) or ne (not equals). The literal_string is the string value to filter to. The literal value must be valid for the type of field you are filtering by (string, number, boolean). For string fields, the literal value is interpreted as a regular expression using RE2 syntax. The literal value must match the entire field.

For example, to filter for instances that do not have a name of example-instance, you would use filter=name ne example-instance.

Compute Engine Beta API Only: If you use filtering in the Beta API, you can also filter on nested fields. For example, you could filter on instances that have set the scheduling.automaticRestart field to true. In particular, use filtering on nested fields to take advantage of instance labels to organize and filter results based on label values.

The Beta API also supports filtering on multiple expressions by providing each separate expression within parentheses. For example, (scheduling.automaticRestart eq true) (zone eq us-central1-f). Multiple expressions are treated as AND expressions, meaning that resources must match all expressions to pass the filters.
* `maxResults` - _optional_ - The maximum number of results per page that should be returned. If the number of available results is larger than maxResults, Compute Engine returns a nextPageToken that can be used to get the next page of results in subsequent list requests.
* `orderBy` - _optional_ - Sorts list results by a certain order. By default, results are returned in alphanumerical order based on the resource name.

You can also sort results in descending order based on the creation timestamp using orderBy="creationTimestamp desc". This sorts results based on the creationTimestamp field in reverse chronological order (newest result first). Use this to sort resources like operations so that the newest operation is returned first.

Currently, only sorting by name or creationTimestamp desc is supported.
* `pageToken` - _optional_ - Specifies a page token to use. Set pageToken to the nextPageToken returned by a previous list request to get the next page of results.
* `project` - _required_ - Project ID for this request.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters. Overrides userIp if both are provided.
* `userIp` - _optional_ - IP address of the site where the request originates. Use this if you want to enforce per-user limits.

### Creates a User resource in the specified project using the data included in the request.

*Tags:* `users`

#### Input Parameters
* `project` - _required_ - Project ID for this request.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters. Overrides userIp if both are provided.
* `userIp` - _optional_ - IP address of the site where the request originates. Use this if you want to enforce per-user limits.

### Gets the access control policy for a resource. May be empty if no such policy or resource exists.

*Tags:* `users`

#### Input Parameters
* `project` - _required_ - Project ID for this request.
* `resource` - _required_ - Name of the resource for this request.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters. Overrides userIp if both are provided.
* `userIp` - _optional_ - IP address of the site where the request originates. Use this if you want to enforce per-user limits.

### Sets the access control policy on the specified resource. Replaces any existing policy.

*Tags:* `users`

#### Input Parameters
* `project` - _required_ - Project ID for this request.
* `resource` - _required_ - Name of the resource for this request.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters. Overrides userIp if both are provided.
* `userIp` - _optional_ - IP address of the site where the request originates. Use this if you want to enforce per-user limits.

### Returns permissions that a caller has on the specified resource.

*Tags:* `users`

#### Input Parameters
* `project` - _required_ - Project ID for this request.
* `resource` - _required_ - Name of the resource for this request.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters. Overrides userIp if both are provided.
* `userIp` - _optional_ - IP address of the site where the request originates. Use this if you want to enforce per-user limits.

### Deletes the specified User resource.

*Tags:* `users`

#### Input Parameters
* `project` - _required_ - Project ID for this request.
* `user` - _required_ - Name of the user resource to delete.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters. Overrides userIp if both are provided.
* `userIp` - _optional_ - IP address of the site where the request originates. Use this if you want to enforce per-user limits.

### Returns the specified User resource.

*Tags:* `users`

#### Input Parameters
* `project` - _required_ - Project ID for this request.
* `user` - _required_ - Name of the user resource to return.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters. Overrides userIp if both are provided.
* `userIp` - _optional_ - IP address of the site where the request originates. Use this if you want to enforce per-user limits.

### Adds a public key to the specified User resource with the data included in the request.

*Tags:* `users`

#### Input Parameters
* `project` - _required_ - Project ID for this request.
* `user` - _required_ - Name of the user for this request.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters. Overrides userIp if both are provided.
* `userIp` - _optional_ - IP address of the site where the request originates. Use this if you want to enforce per-user limits.

### Removes the specified public key from the user.

*Tags:* `users`

#### Input Parameters
* `fingerprint` - _required_ - The fingerprint of the public key to delete. Public keys are identified by their fingerprint, which is defined by RFC4716 to be the MD5 digest of the public key.
* `project` - _required_ - Project ID for this request.
* `user` - _required_ - Name of the user for this request.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters. Overrides userIp if both are provided.
* `userIp` - _optional_ - IP address of the site where the request originates. Use this if you want to enforce per-user limits.

### Returns a list of authorized public keys for a specific user account.

*Tags:* `linux`

#### Input Parameters
* `instance` - _required_ - The fully-qualified URL of the virtual machine requesting the view.
* `login` - _optional_ - Whether the view was requested as part of a user-initiated login.
* `project` - _required_ - Project ID for this request.
* `user` - _required_ - The user account for which you want to get a list of authorized public keys.
* `zone` - _required_ - Name of the zone for this request.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters. Overrides userIp if both are provided.
* `userIp` - _optional_ - IP address of the site where the request originates. Use this if you want to enforce per-user limits.

### Retrieves a list of user accounts for an instance within a specific project.

*Tags:* `linux`

#### Input Parameters
* `filter` - _optional_ - Sets a filter expression for filtering listed resources, in the form filter={expression}. Your {expression} must be in the format: field_name comparison_string literal_string.

The field_name is the name of the field you want to compare. Only atomic field types are supported (string, number, boolean). The comparison_string must be either eq (equals) or ne (not equals). The literal_string is the string value to filter to. The literal value must be valid for the type of field you are filtering by (string, number, boolean). For string fields, the literal value is interpreted as a regular expression using RE2 syntax. The literal value must match the entire field.

For example, to filter for instances that do not have a name of example-instance, you would use filter=name ne example-instance.

Compute Engine Beta API Only: If you use filtering in the Beta API, you can also filter on nested fields. For example, you could filter on instances that have set the scheduling.automaticRestart field to true. In particular, use filtering on nested fields to take advantage of instance labels to organize and filter results based on label values.

The Beta API also supports filtering on multiple expressions by providing each separate expression within parentheses. For example, (scheduling.automaticRestart eq true) (zone eq us-central1-f). Multiple expressions are treated as AND expressions, meaning that resources must match all expressions to pass the filters.
* `instance` - _required_ - The fully-qualified URL of the virtual machine requesting the views.
* `maxResults` - _optional_ - The maximum number of results per page that should be returned. If the number of available results is larger than maxResults, Compute Engine returns a nextPageToken that can be used to get the next page of results in subsequent list requests.
* `orderBy` - _optional_ - Sorts list results by a certain order. By default, results are returned in alphanumerical order based on the resource name.

You can also sort results in descending order based on the creation timestamp using orderBy="creationTimestamp desc". This sorts results based on the creationTimestamp field in reverse chronological order (newest result first). Use this to sort resources like operations so that the newest operation is returned first.

Currently, only sorting by name or creationTimestamp desc is supported.
* `pageToken` - _optional_ - Specifies a page token to use. Set pageToken to the nextPageToken returned by a previous list request to get the next page of results.
* `project` - _required_ - Project ID for this request.
* `zone` - _required_ - Name of the zone for this request.

## License

**flow**ground :- Telekom iPaaS / googleapis-com-clouduseraccounts-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
