---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a92f1fffa0da76d59fd0d992312ce0fc5d014f88e3fd02e1f1bb55fc112cb44a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105811"
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