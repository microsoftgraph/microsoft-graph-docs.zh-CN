---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7762c09c9eb349d52702e611c5725902e3eedc63
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801705"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var trustFrameworkKeySet = await graphClient.TrustFramework.KeySets["{trustFrameworkKeySet-id}"]
    .Request()
    .GetAsync();

```