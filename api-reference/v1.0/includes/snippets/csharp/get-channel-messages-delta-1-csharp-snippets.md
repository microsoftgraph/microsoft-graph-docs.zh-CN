---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 42994a8a6da459cde6e2593d3293ebbedf8e6870
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809289"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chatMessage = await graphClient.Teams["{team-id}"].Channels["{channel-id}"].Messages["{chatMessage-id}"]
    .Request()
    .Top(2)
    .GetAsync();

```