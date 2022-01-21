---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 022f235cd2ff4ae353bcbc8953ac74f8fb391140
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62101283"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    "@odata.id" = "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}

New-MgDeviceRegisteredOwnerByRef -DeviceId $deviceId -BodyParameter $params

```