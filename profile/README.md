# Welcome to IdentityAPI

## Overview

**IdentityAPI** is dedicated to developing robust Django/DRF API applications for managing foundational system functionalities. Our focus lies in providing streamlined solutions for authentication, authorization, and user communication ~ the building blocks of any modern application.

## First, what are the limitations

While managed authentication solutions are robust, they often come with predefined workflows that may not align with specific business requirements. Additionally, these solutions can limit data ownership and typically charge based on the number of users, API requests, or feature tiers—costs that can escalate significantly as your user base grows.

## Second, how IdentityAPI addresses them

**IdentityAPI** introduces ***AAA*** — a family of three Django/DRF applications (*Authen*, *Author*, and *Accord*) that together form a comprehensive system, with each app addressing a specific aspect of functionality. Each application is fully customizable to meet unique business needs. Additionally, the core components can be combined in various configurations to suit different requirements, such as: *Authen* alone, *Authen* with *Author*, *Authen* with *Accord*, or the complete suite of *Authen*, *Author*, and *Accord*.

### Authen  

Handles user authentication and account management, built around a custom user authentication model and a profile model. **Authen** uses [JWT](https://jwt.io/) for secure token-based authentication and ensures minimal data collection to operate effectively. It supports standard user roles (user, staff, admin, and superuser), all of which can be customized to fit specific needs. With features for user registration, login, session handling, and account updates, **Authen** provides a flexible and scalable foundation for managing user identities.  

### Author  

Manages user authorization by leveraging Django’s built-in `Permission` and `Group` models to control access levels and roles. **Author** allows creating and managing custom permissions and groups, enabling fine-grained access control. Each user, permission, or group can be edited individually to meet unique business requirements. This flexibility ensures that organizations can implement robust and tailored access management policies efficiently.  

### Accord  

Facilitates communication between system users with support for real-time notifications and messaging. **Accord** enables:

- One-to-one conversations (e.g., user-to-user, user-to-staff, or user-to-admin).  
- Group conversations (e.g., user-created groups, admin groups, or superuser groups).  
- One-to-group interactions (e.g., a user messaging all admins).  

This app ensures seamless collaboration across various user levels, making it ideal for systems requiring efficient and organized communication.  
