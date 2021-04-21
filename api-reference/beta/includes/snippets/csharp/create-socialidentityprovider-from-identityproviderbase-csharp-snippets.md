---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4b654f066139bec70d5e7b79f0b6642a2b61ee8e
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921312"
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