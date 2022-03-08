---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 867bd2a16b7a3326f56b8cb78d943c06179504cb
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335505"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Administration

$params = @{
    "@odata.type" = "#microsoft.graph.cloudPcUserSetting"
    DisplayName = "Example"
    SelfServiceEnabled = $true
    RestorePointSetting = @{
        FrequencyInHours = "16"
        UserRestoreEnabled = $true
    }
    LocalAdminEnabled = $false
}

Update-MgDeviceManagementVirtualEndpointUserSetting -CloudPcUserSettingId $cloudPcUserSettingId -BodyParameter $params

```