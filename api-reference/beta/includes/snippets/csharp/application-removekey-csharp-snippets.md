---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ccad3f01d799538972a9860214d43adeaf99e9f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784495"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var keyId = Guid.Parse("f0b0b335-1d71-4883-8f98-567911bfdca6");

var proof = "eyJ0eXAiOiJ...";

await graphClient.Applications["{application-id}"]
    .RemoveKey(keyId,proof)
    .Request()
    .PostAsync();

```