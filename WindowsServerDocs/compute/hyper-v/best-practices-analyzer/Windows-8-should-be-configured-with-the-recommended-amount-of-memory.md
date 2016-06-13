---
title: Windows 8 should be configured with the recommended amount of memory
ms.custom: na
ms.prod: windows-server-threshold
ms.reviewer: na
ms.suite: na
ms.technology: 
  - hyper-v
  - techgroup-compute
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 0c739e7c-4403-4eff-9e69-213ba1ab7336
author: KBDAzure
---
# Windows 8 should be configured with the recommended amount of memory
\[This information is preliminary and subject to change.  
  
For more information about best practices and scans, see [Run Best Practices Analyzer Scans and Manage Scan Results](http://go.microsoft.com/fwlink/p/?LinkID=223177).  
  
|||  
|-|-|  
|**Operating System**|Windows Server 2016 Technical Preview|  
|**Product\/Feature**|Hyper\-V|  
|**Severity**|Warning|  
|**Category**|Configuration|  
  
  
  
The following sections provide details about the specific issue. Italics indicates UI text that appears in the Best Practices Analyzer tool for the specific issue.  
  
## **Issue**  
*A virtual machine running Windows 8 is configured with less than the recommended amount of RAM, which is 1 GB.*  
  
## **Impact**  
*The guest operating system and applications might not perform well. There might not be enough memory to run multiple applications at once. This impacts the following virtual machines:*  
```  
<list of virtual machines>  
```  
## **Resolution**  
*Use Hyper\-V Manager to increase the memory allocated to this virtual machine to at least 1 GB.*  
  
### Increase the memory using Hyper\-V Manager  
  
1.  Open Hyper\-V Manager. Click **Start**, point to **Administrative Tools**, and then click **Hyper\-V Manager**.  
  
2.  In the results pane, under **Virtual Machines**, select the virtual machine that you want to configure. The state of the virtual machine should be listed as **Off**. If it is not, right\-click the virtual machine and then click **Shut Down**.  
  
3.  In the **Action** pane, under the virtual machine name, click **Settings**.  
  
4.  In the navigation pane, click **Memory**.  
  
5.  On the **Memory** page, set the **Startup RAM** to at least 1 GB and then click **OK**.  
  
### Increase the memory using Windows PowerShell  
  
1.  Open Windows PowerShell. \(From the desktop, click **Start** and start typing **Windows PowerShell**.\)  
  
2.  Right\-click **Windows PowerShell** and click **Run as administrator**.  
  
3.  Run this command after replacing \<MyVM> with the name  of your virtual machine:  
  
```  
Set-VMMemory <MyVM> -StartupBytes 1GB  
```  
  
## See Also  
[Set-VMMemory](https://technet.microsoft.com/library/hh848572.aspx)  
  
