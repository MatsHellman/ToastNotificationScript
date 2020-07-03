# ToastNotificationScript
The Windows 10 Toast Notification Script enables you to create nice and nifty toast notifications for the logged on user in Windows 10.  
This script is a branch of Martin Bengtssons script found here, https://www.imab.dk/windows-10-toast-notification-script/ all credit to him for creating the whole system. My branch is a copy to work when using Windows 10 Servicing and getting the DynamicDeadline information from WMI. On top of that I have some ideas on how to improve it for my users.  
My changes will ofcourse be presented to Martin in case he want's to implement them in his sript as well. The license model is kept as Martin had his, as a MIT license. 
## Added functions
### Dynamic Deadline for servicing updates 
To use the Servicing update instead of the task sequence deadline you need to  
- [ ] Set the OsUpgradeType Update (tasksequence for the traditional functionality)
- [ ] Define the UpdateID you can find in your update information in the ConfigMGR console to %___AND_THE_ID. The precent sign is important, otherwise the WQL query will fail.
Everything else is still as Martin defined it in the original scripts when looking at settings.

## Ideas to add to the scripts
- [x] Ability to find the servicing updates deadline dynamically
- [ ] Logic in script to handle localization
  - [ ] Create localized verision of xml
  - [ ] Ability to read the computer or user localization settings

