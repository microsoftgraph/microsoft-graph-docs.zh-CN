---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6cfa5d9a55a06e6cad9b4865bc166c4a67bc6c8e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893166"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = new Group
{
    Description = "Group with designated owner and members",
    DisplayName = "Operations group",
    GroupTypes = new List<String>()
    {
        "Unified"
    },
    MailEnabled = true,
    MailNickname = "operations2019",
    SecurityEnabled = false,
    AdditionalData = new Dictionary<string, object>()
    {
        {"members@odata.bind",["https://graph.microsoft.com/v1.0/users/ff7cb387-6688-423c-8188-3da9532a73cc","https://graph.microsoft.com/v1.0/users/69456242-0067-49d3-ba96-9de6f2728e14"]},
        {"owners@odata.bind",["https://graph.microsoft.com/v1.0/users/26be1845-4119-4801-a799-aea79d09f1a2"]}
    }
};

await graphClient.Groups
    .Request()
    .AddAsync(group);

```