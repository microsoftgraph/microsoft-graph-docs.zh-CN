---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 90f676743936ffb212ade709f6b05fbe93d6c3ab
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778428"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var posts = await graphClient.Groups["{group-id}"].Threads["{conversationThread-id}"].Posts
    .Request()
    .GetAsync();

```