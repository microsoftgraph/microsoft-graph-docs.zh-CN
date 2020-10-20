---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 268f21e78095874ec41dfa63d0bed37e825961c6
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48620547"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityProvider = new IdentityProvider
{
    Name = "Login with Amazon",
    Type = "Amazon",
    ClientId = "56433757-cadd-4135-8431-2c9e3fd68ae8",
    ClientSecret = "000000000000"
};

await graphClient.IdentityProviders
    .Request()
    .AddAsync(identityProvider);

```