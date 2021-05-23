# PSAnsibleHelperFunctions4Linux
This is a PowerShell  module exclusively for Linux for development for Ansible modules that will be run on Linux.
The reason why there is no Windows Support is because Ansible already provides a mechanism to have these cmdlets available in using Ansible modules for Windows. The use of this functions and how to call and write in Windows can be documented [here](https://docs.ansible.com/ansible/2.6/dev_guide/developing_modules_general_windows.html). 

Please note on Linux using module_utils is not an option because it calls the shebang !#powershell which causes problems. #Requires does not work well because of the above reason as well. This module seeks to resolve that issue by putting in the necessary functions in a custom module which you can then call. 
These are taken straight from the Ansible library. They are not using approved verbs. Currently keeping these consistent with the Ansible notes.
