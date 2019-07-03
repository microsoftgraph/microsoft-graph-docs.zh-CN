---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b3770987fc63ab1191a8c84e93c85bca27af0d14
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35521212"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedRoleSettings = new PrivilegedRoleSettings
{
    Id = "9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3",
    ElevationDuration = "PT8H",
    NotificationToUserOnElevation = false,
    TicketingInfoOnElevation = true,
    MfaOnElevation = false,
    MaxElavationDuration = "PT0S",
    MinElevationDuration = "PT0S",
    LastGlobalAdmin = false,
    IsMfaOnElevationConfigurable = true,
    ApprovalOnElevation = false,
    ApproverIds = new List<String>()
    {
        "e2b2a2fb-13d7-495c-adc9-941fe966793f",
        "22770e3f-b9b4-418e-9dea-d0e3d2f275dd"
    }
};

await graphClient.PrivilegedRoles["{id}"].Settings
    .Request()
    .PutAsync(privilegedRoleSettings);

```