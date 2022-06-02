---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 13aaf5305e64cdce8728aaffb106ff7e7c638608
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/01/2022
ms.locfileid: "65828762"
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

Invoke-MgBulkRestoreDeviceManagementManagedDeviceCloudPc -BodyParameter $params

```