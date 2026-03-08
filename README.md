# Password Manager 3
_Made in QB64_  
A password manager made to store passwords, backup codes, totp codes, and an extra type of code.

# Features
* Can store credentials for many accounts
* Can store four types of codes for each account
* Can store a list of backup codes
* Encrypted File: any user can encrypt and add entries, with no way for others to decrypt it
* Has built-in command line arguments' scripting enabled: User can provide a list of commands in the command prompt
* Multi-authentication system: users can unlock using Password / Pin, both giving different privileges to users
* Decrypted sessions: users can work on unlocked vault for atmost a certain time

# Syntax
pwdmgr3 \[Session Management\] \[Commands\] \[Attributes\] \[Options\] \[Arguments\]

## Session Management
* pwd - Password
* pin - Pin
* new\_pwd - Set a new Password
* new\_pin - Set a new Pin
* lock - Forcefully lock the session, even before the time is up.
_Will implement Totp unlocking later_

## Commands
* add - Add an account entry
* insert - Insert an account entry at a specified position
* list - List all accounts
* view\_everything - View all accounts and there attributes
* select - Select an account by ID to operate on it's attributes
* select\_find - Select an account by Finding
* rename - Rename an account identifier
* delete - Delete an account entry

## Attributes
* password - Operate on Password
* backup\_code - Operate on List of Backup Codes
* totp - Operate on TOTP Code
* extra - Operate on Extra Code

## Options
* create - Create a random string, useful for creating a random password
* set - Set/add an attribute's value
* load - Load an attribute's value from text file
* remove / clear - Clear an attribute's value
* peek - Peek an attribute's value, do not delete anything
* view - View an attribute's value and then delete the current Backup Code, if a backup code is viewed
* copy - Copy an attribute's value to system clipboard
