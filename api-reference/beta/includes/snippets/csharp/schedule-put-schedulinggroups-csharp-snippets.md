---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 138ac4891bb857d9196451250e23f66f75f8b2b8
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48620397"
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