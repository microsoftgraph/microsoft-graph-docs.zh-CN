---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a3732a1b0f6dbd844783d4217ff9cdc2747968d3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800058"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var temporaryAccessPassAuthenticationMethod = new TemporaryAccessPassAuthenticationMethod
{
    StartDateTime = DateTimeOffset.Parse("2021-01-26T00:00:00Z"),
    LifetimeInMinutes = 60,
    IsUsableOnce = false
};

await graphClient.Users["{user-id}"].Authentication.TemporaryAccessPassMethods
    .Request()
    .AddAsync(temporaryAccessPassAuthenticationMethod);

```