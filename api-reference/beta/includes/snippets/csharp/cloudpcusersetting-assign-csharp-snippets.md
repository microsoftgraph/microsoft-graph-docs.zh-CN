---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: af3d1cdd8389f3768bba6c52965e0dd610879ad2
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207110"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var assignments = new List<CloudPcUserSettingAssignment>()
{
    new CloudPcUserSettingAssignment
    {
        Id = "b0c2d35f-3385-46c8-a6f5-6c3dfad7708b_64ff06de-9c00-4a5a-98b5-7f5abe26ffff",
        Target = new CloudPcManagementGroupAssignmentTarget
        {
            GroupId = "64ff06de-9c00-4a5a-98b5-7f5abe26ffff"
        }
    }
};

await graphClient.DeviceManagement.VirtualEndpoint.UserSettings["{cloudPcUserSetting-id}"]
    .Assign(assignments)
    .Request()
    .PostAsync();

```