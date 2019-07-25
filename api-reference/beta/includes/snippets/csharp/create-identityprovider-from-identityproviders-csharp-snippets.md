---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 268f21e78095874ec41dfa63d0bed37e825961c6
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35711612"
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