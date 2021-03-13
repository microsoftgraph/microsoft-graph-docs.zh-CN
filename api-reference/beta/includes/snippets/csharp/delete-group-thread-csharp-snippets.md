---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 35ddc9f6065de71f75df80c00d54e9a881b3bbc9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793455"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{group-id}"].Threads["{conversationThread-id}"]
    .Request()
    .DeleteAsync();

```