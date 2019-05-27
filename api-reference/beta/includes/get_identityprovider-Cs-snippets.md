---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 422ee8dc95bdc2a0c3c6234fd2c9f5d7228fdb70
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34449473"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityProvider = await graphClient.IdentityProviders["Amazon-OAuth"]
    .Request()
    .GetAsync();

```