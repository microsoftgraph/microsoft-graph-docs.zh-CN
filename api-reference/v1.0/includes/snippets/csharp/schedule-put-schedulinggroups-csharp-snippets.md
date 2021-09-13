---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d5bd33229087515852a4469a1405e72466132a4f2c17088d2dba35fe85558554
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158400"
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

await graphClient.Teams["{team-id}"].Schedule.SchedulingGroups["{schedulingGroup-id}"]
    .Request()
    .Header("Prefer","return=representation")
    .PutAsync(schedulingGroup);

```