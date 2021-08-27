---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3ff65bd432ce75869f8c95174b6bd6c4c954fb3ef78d1ca5c31fbebcc65765d8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105388"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityProviderBase = new SocialIdentityProvider
{
    DisplayName = "Login with Amazon",
    IdentityProviderType = "Amazon",
    ClientId = "56433757-cadd-4135-8431-2c9e3fd68ae8",
    ClientSecret = "000000000000"
};

await graphClient.Identity.IdentityProviders
    .Request()
    .AddAsync(identityProviderBase);

```