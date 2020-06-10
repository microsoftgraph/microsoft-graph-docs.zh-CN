---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7e48ac3c4398fce0cbc91ca3a2221e4c0e7b5ee0
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44683847"
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

await graphClient.PrivilegedRoles["{id}"].Settings
    .Request()
    .PutAsync(privilegedRoleSettings);

```