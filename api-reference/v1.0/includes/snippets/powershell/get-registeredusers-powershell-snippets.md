---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1831ff1eb5aa38777b8cfbbafde2ed0a943e362c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62101311"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

Get-MgDeviceRegisteredUser -DeviceId $deviceId

```