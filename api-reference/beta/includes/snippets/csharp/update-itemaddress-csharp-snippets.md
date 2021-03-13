---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b36e4758352540cd3eae407b88aa66fcf2e21c7c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774676"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var itemAddress = new ItemAddress
{
    AllowedAudiences = AllowedAudiences.Me,
    DisplayName = "Secret Hideout"
};

await graphClient.Users["{user-id}"].Profile.Addresses["{itemAddress-id}"]
    .Request()
    .UpdateAsync(itemAddress);

```