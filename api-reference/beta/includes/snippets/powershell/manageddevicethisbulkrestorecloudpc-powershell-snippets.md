---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 04e251ceae4adf8b0a721701965094114188a9d4
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338191"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Actions

$params = @{
    ManagedDeviceIds = @(
        "30d0e128-de93-41dc-89ec-33d84bb662a0"
        "7c82a3e3-9459-44e4-94d9-b92f93bf78dd"
    )
    RestorePointDateTime = [System.DateTime]::Parse("2021-09-23T04:00:00.0000000")
    TimeRange = "before"
}

Invoke-MgBulkDeviceManagementManagedDeviceRestoreCloudPc -BodyParameter $params

```