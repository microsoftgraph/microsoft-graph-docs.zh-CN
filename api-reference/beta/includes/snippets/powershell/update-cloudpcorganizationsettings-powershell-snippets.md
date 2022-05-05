---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eb066c19fc327807ce5a602294298815be13dc94
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65220282"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Administration

$params = @{
    "@odata.type" = "#microsoft.graph.cloudPcOrganizationSettings"
    UserAccountType = "standardUser"
    OsVersion = "windows11"
    WindowsSettings = @{
        Language = "en-US"
    }
}

Update-MgDeviceManagementVirtualEndpointOrganizationSetting -BodyParameter $params

```