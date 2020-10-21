---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 422ee8dc95bdc2a0c3c6234fd2c9f5d7228fdb70
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48621345"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityProvider = await graphClient.IdentityProviders["Amazon-OAuth"]
    .Request()
    .GetAsync();

```