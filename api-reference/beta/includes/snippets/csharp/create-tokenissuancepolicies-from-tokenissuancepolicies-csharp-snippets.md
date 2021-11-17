---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4179123d632fed6944f08b1c95d44c5d56d307769e13494fbe7459bbc5e408ea
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903609"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tokenIssuancePolicy = new TokenIssuancePolicy
{
    Definition = new List<String>()
    {
        "definition-value"
    },
    DisplayName = "displayName-value",
    IsOrganizationDefault = true
};

await graphClient.Policies.TokenIssuancePolicies
    .Request()
    .AddAsync(tokenIssuancePolicy);

```