---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 730433e04b57b0cb8b8844f71599802f46f5bad2
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "47329722"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityProviders = await graphClient.Identity.B2cUserFlows["{id}"].IdentityProviders
    .Request()
    .GetAsync();

```