---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 44bc8f57842917e2738d4ecdaa063b48c88a017f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810252"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var subscribedSku = await graphClient.SubscribedSkus["{subscribedSku-id}"]
    .Request()
    .GetAsync();

```