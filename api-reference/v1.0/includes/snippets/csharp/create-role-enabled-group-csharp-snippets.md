---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e61e8aa216e0173602130f2cd2330eaf15ca8150
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59998184"
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
        {"owners@odata.bind", "[\"https://graph.microsoft.com/v1.0/users/99e44b05-c10b-4e95-a523-e2732bbaba1e\"]"},
        {"members@odata.bind", "[\"https://graph.microsoft.com/v1.0/users/6ea91a8d-e32e-41a1-b7bd-d2d185eed0e0\",\"https://graph.microsoft.com/v1.0/users/4562bcc8-c436-4f95-b7c0-4f8ce89dca5e\"]"}
    }
};

await graphClient.Groups
    .Request()
    .AddAsync(group);

```