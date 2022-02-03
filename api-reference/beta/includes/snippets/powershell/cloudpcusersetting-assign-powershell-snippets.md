---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 48d7ddb974ad760808535579d0586b4adcc69653
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62339887"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Actions

$params = @{
    Assignments = @(
        @{
            Id = "b0c2d35f-3385-46c8-a6f5-6c3dfad7708b_64ff06de-9c00-4a5a-98b5-7f5abe26ffff"
            Target = @{
                "@odata.type" = "microsoft.graph.cloudPcManagementGroupAssignmentTarget"
                GroupId = "64ff06de-9c00-4a5a-98b5-7f5abe26ffff"
            }
        }
    )
}

Set-MgDeviceManagementVirtualEndpointUserSetting -CloudPcUserSettingId $cloudPcUserSettingId -BodyParameter $params

```