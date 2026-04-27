##Federation:
•	Occurs when an external Identity provider (IdP) authenticate access on behalf of Microsoft Entra ID. The IdP validates the users’ credentials and issue a security token back to Microsoft Entra ID. 
•	There is a Trust Relationship between Entra ID and the external IdP. The IdP manages user credentials and sends a token to Entra ID when the authentication is validated. Entra ID trusts the token (common with protocols such AD FS, SAML and OIDC)
•	This trust relationship means the user can sign in to Microsoft Entra-based services using an external password. 
Examples: An organization can enable Federation between their on-premises to cloud. Employees would have access to on cloud resources using their corporate credentials, without the need to have their passwords stored on cloud systems.

##RBAC vs ABAC:
•	In Microsoft Entra ID, Role-based Access Control and Attribute-based Access Control are two mechanisms employed to manage access to corporation resources. RBAC manages access based on job titles and ABAC provide a more granular approach to evaluating users’ access. 
•	Role-Based Access Control (RBAC) assign permissions based on job roles. Permissions are grouped into a job role and assigned to users belonging to the specific group. Rules are built in and can be combined from a pre-defined list to create specific rules for a team for example. 
•	Attribute-Based Access Control (ABAC) adds a layer to the RBAC capabilities. ABAC adds conditions that allow or deny user access to resources. Access is given only if the conditions are met at the time of access. A condition could be the time and location of access, or if the user has access to a given project or department; e.g., only allow access to Finance app if Department=Finance AND device is compliant. 
•	In summary RBAC vs ABAC: RBAC = role grants; ABAC = role + conditions/attributes (often enforced via resource attributes and policy. 
