---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cbd970f2a98611906c43a2d5c48440cfe8639fad
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996433"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.Me.OnlineMeetings["{onlineMeeting-id}"].Recording
    .Request()
    .GetAsync();

```