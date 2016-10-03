---
ms.assetid: c50ecc6a-9504-4b4a-816f-e762dcf3a95e
title: Install the Federation Service Proxy Role Service
description:
author: billmath
manager: femila
ms.date: 09/21/2016
ms.topic: article
ms.prod: windows-server-threshold
ms.service: active-directory
ms.technology: identity-adfs
ms.author: billmath
---

# Install the Federation Service Proxy Role Service

>Applies To: Windows Server 2016, Windows Server 2012 R2, Windows Server 2012

After you configure a computer with the prerequisite applications and certificates, you are ready to install the Federation Service Proxy role service of Active Directory Federation Services \(AD FS\). You can use the following procedure to install the Federation Service Proxy role service. When you install the Federation Service Proxy role service on a computer, that computer becomes a federation server proxy.  
  
Membership in **Administrators**, or equivalent, on the local computer is the minimum required to complete this procedure.  Review details about using the appropriate accounts and group memberships at [Local and Domain Default Groups](http://go.microsoft.com/fwlink/?LinkId=83477).   
  
### To install the Federation Service Proxy role service  
  
1.  On the **Start** screen, type**Server Manager**, and then press ENTER.  
  
2.  Click **Manage**, and then click **Add Roles and Features** to start the Add Roles and Features Wizard.  
  
3.  On the **Before you begin** page, click **Next**.  
  
4.  On the **Select installation type** page, click **Role\-based or Feature\-based installation**, and click **Next**.  
  
5.  On the **Select destination server** page, click **Select a server from the server pool**, verify that the target computer is highlighted, and then click **Next**.  
  
6.  On the **Select server roles** page, click **Active Directory Federation Services**, and then click next.  
  
    > [!NOTE]  
    > If you are prompted to install additional .NET Framework or Windows Process Activation Service features, click **Add Features** to install them.  
  
7.  On the **Select features** page, verify that the features are set, and then click **Next**.  
  
8.  On the **Active Directory Federation Service \(AD FS\)** page, click **Next**.  
  
9. On the **Select role services** page, select the **Federation Service Proxy** check box, and then click **Next**.  
  
10. On the **Web Server Role \(IIS\)** page, click **Next**.  
  
11. On the **Select role services** page, click **Next**.  
  
12. After you verify the information on the **Confirm installation selections** page, select the **Restart the destination server automatically if required** check box, and then click **Install**.  
  
13. On the **Installation progress** page, verify that everything installed correctly, and then click **Close**.  
  
## Additional references  
[Checklist: Setting Up a Federation Server](Checklist--Setting-Up-a-Federation-Server.md)  
  
[Checklist: Setting Up a Federation Server Proxy](Checklist--Setting-Up-a-Federation-Server-Proxy.md)  
  
