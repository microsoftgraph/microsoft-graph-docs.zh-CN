---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8584707b374f4d99aed0545b030a83d910116c1d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794901"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedRoleSettings = new PrivilegedRoleSettings
{
    Id = "9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3",
    ElevationDuration = new Duration("PT8H"),
    NotificationToUserOnElevation = false,
    TicketingInfoOnElevation = true,
    MfaOnElevation = false,
    MaxElavationDuration = new Duration("PT0S"),
    MinElevationDuration = new Duration("PT0S"),
    LastGlobalAdmin = false,
    IsMfaOnElevationConfigurable = true,
    ApprovalOnElevation = false,
    ApproverIds = new List<String>()
    {
        "e2b2a2fb-13d7-495c-adc9-941fe966793f",
        "22770e3f-b9b4-418e-9dea-d0e3d2f275dd"
    }
};

await graphClient.PrivilegedRoles["{privilegedRole-id}"].Settings
    .Request()
    .PutAsync(privilegedRoleSettings);

```