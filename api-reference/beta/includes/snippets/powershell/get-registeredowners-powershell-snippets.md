---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8197c2ff15745a3a2fb5f1474be7e10bfb335462
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62106366"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

Get-MgDeviceRegisteredOwner -DeviceId $deviceId

```