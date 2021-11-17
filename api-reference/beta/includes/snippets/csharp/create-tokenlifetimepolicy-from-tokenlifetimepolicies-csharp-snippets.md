---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a0a67c35975f4845f1a3a02b1d19ebad12f6b1bcf9e8ec17c26511fa8bde9aaa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903284"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tokenLifetimePolicy = new TokenLifetimePolicy
{
    Definition = new List<String>()
    {
        "definition-value"
    },
    DisplayName = "displayName-value",
    IsOrganizationDefault = true
};

await graphClient.Policies.TokenLifetimePolicies
    .Request()
    .AddAsync(tokenLifetimePolicy);

```