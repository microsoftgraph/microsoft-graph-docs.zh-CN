---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 062cc7336bc65bf439dc2e4b4d94f85b54ca478a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62092526"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

Get-MgDeviceTransitiveMemberOf -DeviceId $deviceId

```