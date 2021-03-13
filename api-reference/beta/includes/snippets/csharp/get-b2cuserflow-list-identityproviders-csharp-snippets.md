---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5504f9f265df5d598defe70f9abeca87bdd98c32
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797495"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityProviders = await graphClient.Identity.B2cUserFlows["{b2cIdentityUserFlow-id}"].IdentityProviders
    .Request()
    .GetAsync();

```