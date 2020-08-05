---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5c5ca155efe9ae4163657b1e7ccbcdeb7191707e
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46570184"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userIds = new List<String>()
{
    "29f270bb-4d23-4f68-8a57-dc73dc0d4caf"
};

await graphClient.IdentityProtection.RiskyUsers
    .ConfirmCompromised(userIds)
    .Request()
    .PostAsync();

```