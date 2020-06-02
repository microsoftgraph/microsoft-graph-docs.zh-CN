---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 138ac4891bb857d9196451250e23f66f75f8b2b8
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "35725604"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schedulingGroup = new SchedulingGroup
{
    DisplayName = "Cashiers",
    IsActive = true,
    UserIds = new List<String>()
    {
        "c5d0c76b-80c4-481c-be50-923cd8d680a1",
        "2a4296b3-a28a-44ba-bc66-0274b9b95851"
    }
};

await graphClient.Teams["{teamId}"].Schedule.SchedulingGroups["{schedulingGroupId}"]
    .Request()
    .Header("Prefer","return=representation")
    .PutAsync(schedulingGroup);

```