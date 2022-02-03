---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1151bc7e0bc84e927c578eef50fb0187d0eeed42
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62341226"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Actions

$params = @{
    UserAccountType = "administrator"
    OsVersion = "windows10"
}

Invoke-MgReprovisionDeviceManagementVirtualEndpointCloudPc -CloudPCId $cloudPCId -BodyParameter $params

```