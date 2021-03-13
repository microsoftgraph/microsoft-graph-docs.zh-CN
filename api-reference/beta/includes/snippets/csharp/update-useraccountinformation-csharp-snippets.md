---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2638dc3b5d37eb6ce285e226a4b2e070d7aa13c0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787519"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userAccountInformation = new UserAccountInformation
{
    CountryCode = "NO"
};

await graphClient.Me.Profile.Account["{userAccountInformation-id}"]
    .Request()
    .UpdateAsync(userAccountInformation);

```