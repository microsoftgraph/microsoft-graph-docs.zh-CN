---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7279f81afd07a338e74c01fb3f8b99bbde0422b51deb2d02c1fdb5f1804917c6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278537"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = new Group
{
    Description = "Group with designated owner and members",
    DisplayName = "Operations group",
    GroupTypes = new List<String>()
    {
    },
    MailEnabled = false,
    MailNickname = "operations2019",
    SecurityEnabled = true,
    AdditionalData = new Dictionary<string, object>()
    {
        {"owners@odata.bind", "[\"https://graph.microsoft.com/v1.0/users/26be1845-4119-4801-a799-aea79d09f1a2\"]"},
        {"members@odata.bind", "[\"https://graph.microsoft.com/v1.0/users/ff7cb387-6688-423c-8188-3da9532a73cc\",\"https://graph.microsoft.com/v1.0/users/69456242-0067-49d3-ba96-9de6f2728e14\"]"}
    }
};

await graphClient.Groups
    .Request()
    .AddAsync(group);

```