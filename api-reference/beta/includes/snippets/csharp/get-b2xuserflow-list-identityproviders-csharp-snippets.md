---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c57dab08cb1b4728c4aef8ca3437fb21b7fbe6bf
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "47329383"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityProviders = await graphClient.Identity.B2xUserFlows["{id}"].IdentityProviders
    .Request()
    .GetAsync();

```