---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 26284be4492fc5ecbb3bedc5fd8cdaf6f67695c5
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62106352"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    "@odata.id" = "https://graph.microsoft.com/beta/directoryObjects/{id}"
}

New-MgDeviceRegisteredUserByRef -DeviceId $deviceId -BodyParameter $params

```