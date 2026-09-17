# Windows Server & Active Directory Lab

## Project Overview

This is a hands-on Windows Server and Active Directory lab built in Microsoft Azure.

The purpose of this project was to gain practical experience with Windows Server administration, Active Directory, user and group management, DNS, and PowerShell.

This lab simulates a small business Windows domain environment and demonstrates common tasks that are relevant to entry-level IT Support, Help Desk, Desktop Support, and Junior Systems Administration roles.

## Lab Environment

- Microsoft Azure
- Windows Server 2025 Datacenter: Azure Edition
- Active Directory Domain Services (AD DS)
- Windows Server DNS
- Windows PowerShell
- Active Directory PowerShell Module
- Azure Virtual Network
- Domain: `monroetech.local`
- Server: `MonroeLab-tech`

## Technologies & Skills

- Windows Server 2025
- Active Directory
- Active Directory Users and Computers (ADUC)
- DNS
- PowerShell
- Organizational Units (OUs)
- User account administration
- Security groups
- Password management
- Account enable/disable procedures
- Microsoft Azure
- Basic networking concepts

## Active Directory Configuration

The Windows Server was configured as a Domain Controller for the `monroetech.local` domain.

The following Organizational Units were created:

- IT
- HR
- Sales
- Help Desk

A security group named `IT-Support` was created for the IT environment.

A test user account named `Jordan Smith` was created with the username `jsmith`.

Jordan Smith was added to the `IT-Support` security group.

## User Account Administration

I practiced several common Active Directory account-management tasks:

- Created a test user account
- Created and configured a security group
- Added a user to a security group
- Reset a user password
- Disabled a user account
- Verified the account status using PowerShell
- Re-enabled the user account
- Verified the account was active again

PowerShell was used to verify the account status:

`Get-ADUser jsmith -Properties Enabled`

The account was successfully verified as disabled:

`Enabled : False`

The account was then re-enabled and verified:

`Enabled : True`

## PowerShell Administration

PowerShell was used to interact with and verify Active Directory information.

Examples of commands used during the lab include:

`Get-ADUser jsmith`

`Get-ADUser jsmith -Properties Enabled`

`Enable-ADAccount jsmith`

The Active Directory PowerShell module was also verified on the Windows Server.

## What I Practiced

This lab gave me hands-on practice with:

- Domain Controller configuration
- Active Directory administration
- User account management
- Security group management
- Organizational Units
- DNS configuration
- PowerShell
- Account troubleshooting
- Basic Windows Server administration

## Screenshots

Screenshots documenting the lab will be added below.

### Server Manager

Windows Server showing Active Directory Domain Services and DNS.

### Domain Configuration

Windows Server showing the `MonroeLab-tech` server and `monroetech.local` domain.

### Active Directory Organizational Units

Active Directory Users and Computers showing the organizational structure created for the lab.

### IT User and Security Group

The IT organizational structure showing the test user and `IT-Support` security group.

### Security Group Membership

The `IT-Support` security group showing Jordan Smith as a member.

### Disabled Account Verification

PowerShell showing the test account with:

`Enabled : False`

### Re-enabled Account Verification

PowerShell showing the test account with:

`Enabled : True`

## What I Learned

This project helped me develop a better understanding of how Windows Server and Active Directory work together in a domain environment.

I gained practical experience creating users and security groups, organizing users with Organizational Units, managing account access, working with DNS, and using PowerShell to perform administrative tasks and verify account status.

## Future Improvements

I plan to continue expanding this lab by:

- Adding a Windows client machine to the domain
- Practicing Group Policy management
- Creating additional PowerShell automation
- Building networking scenarios
- Practicing DNS troubleshooting
- Adding additional help desk troubleshooting scenarios
- Documenting common Active Directory troubleshooting procedures

## Career Goal

I am using this project to build practical IT skills while pursuing my Information Technology degree.

My goal is to continue developing my skills in IT Support, Help Desk, Networking, Systems Administration, and eventually Network Infrastructure and Cybersecurity.