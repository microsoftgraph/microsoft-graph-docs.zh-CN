---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2b2cb18c070d7308bc7bb9f7981778fca84276df
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62346515"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Actions

$params = @{
    TargetServicePlanId = "30d0e128-de93-41dc-89ec-33d84bb662a0"
}

Resize-MgDeviceManagementManagedDeviceCloudPc -ManagedDeviceId $managedDeviceId -BodyParameter $params

```