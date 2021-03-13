---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 476f14dfb33b1d702b3673bfb1c95c1373f75d5f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787338"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversationThread = await graphClient.Groups["{group-id}"].Threads["{conversationThread-id}"]
    .Request()
    .GetAsync();

```