---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 99647719e322b772cef6eb64a687214e4b3d37e5
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59998179"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = new Group
{
    Description = "Group assignable to a role",
    DisplayName = "Role assignable group",
    GroupTypes = new List<String>()
    {
        "Unified"
    },
    IsAssignableToRole = true,
    MailEnabled = true,
    SecurityEnabled = true,
    MailNickname = "contosohelpdeskadministrators",
    AdditionalData = new Dictionary<string, object>()
    {
        {"owners@odata.bind", "[\"https://graph.microsoft.com/beta/users/99e44b05-c10b-4e95-a523-e2732bbaba1e\"]"},
        {"members@odata.bind", "[\"https://graph.microsoft.com/beta/users/6ea91a8d-e32e-41a1-b7bd-d2d185eed0e0\",\"https://graph.microsoft.com/beta/users/4562bcc8-c436-4f95-b7c0-4f8ce89dca5e\"]"}
    }
};

await graphClient.Groups
    .Request()
    .AddAsync(group);

```