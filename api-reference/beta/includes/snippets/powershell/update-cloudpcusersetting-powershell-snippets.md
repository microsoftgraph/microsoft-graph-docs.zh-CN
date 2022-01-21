---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ab81177a23372a36c95bdc9adf14d3ba825befc3
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62109230"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Administration

$params = @{
    "@odata.type" = "#microsoft.graph.cloudPcUserSetting"
    DisplayName = "Example"
    SelfServiceEnabled = $true
    LocalAdminEnabled = $false
}

Update-MgDeviceManagementVirtualEndpointUserSetting -CloudPcUserSettingId $cloudPcUserSettingId -BodyParameter $params

```