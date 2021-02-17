---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a646b46c68042cca5e2a62370d3c7c4ba671ead6
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50274856"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityUserFlow = new IdentityUserFlow
{
    Id = "Pol1",
    UserFlowType = UserFlowType.SignUpOrSignIn,
    UserFlowTypeVersion = 1f
};

await graphClient.Identity.UserFlows
    .Request()
    .AddAsync(identityUserFlow);

```