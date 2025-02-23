# AWS IAM (Identity and Access Management)

## Introduction to AWS IAM
AWS Identity and Access Management (IAM) is a service that helps securely control access to AWS resources. It enables users to manage permissions, authentication, and policies to ensure security within an AWS environment.

## Key Features of IAM
User Management – Create and manage IAM users and their permissions.
Group Management – Organize users into groups for easier access control.
Role-Based Access – IAM roles allow temporary access to AWS services.
Policy-Based Control – Define fine-grained permissions using JSON-based policies.
Multi-Factor Authentication (MFA) – Adds an extra layer of security.
Federated Access – Use external identity providers (Google, Okta, etc.) for authentication.
Least Privilege Access – Follows best practices to grant only necessary permissions.

## IAM Components
1. IAM Users
    Represents an individual who interacts with AWS.
    Users have unique credentials (username, password, and access keys).
    Can be assigned permissions directly or through groups.

2. IAM Groups
    A collection of IAM users with shared permissions.
    Example: "Developers" group with access to EC2, "Admins" group with full access.

3. IAM Roles
    Used to grant temporary permissions to users, services, or applications.
    Roles do not have static credentials; instead, they are assumed by entities when needed.
    Example: EC2 instance assuming an S3 access role instead of storing access keys.

4. IAM Policies
    JSON-based documents that define permissions for users, groups, and roles.
    Types of Policies:
      AWS Managed Policies – Predefined by AWS.
      Customer Managed Policies – Created and customized by users.
      Inline Policies – Attached directly to a single user, group, or role.