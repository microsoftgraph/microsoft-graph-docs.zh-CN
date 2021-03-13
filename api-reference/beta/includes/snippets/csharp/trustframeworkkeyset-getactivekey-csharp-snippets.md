---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 23591f42bfb7d2b0d3c822d02589a1a9b4718a7d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792612"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var trustFrameworkKey = await graphClient.TrustFramework.KeySets["{trustFrameworkKeySet-id}"]
    .GetActiveKey()
    .Request()
    .GetAsync();

```