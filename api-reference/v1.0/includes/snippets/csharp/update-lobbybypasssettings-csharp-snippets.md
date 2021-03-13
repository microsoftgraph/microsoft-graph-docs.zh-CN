---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6b3eb2d85c6c5d61dd3f4ab3cb013eb20c8f3348
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773513"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var onlineMeeting = new OnlineMeeting
{
    LobbyBypassSettings = new LobbyBypassSettings
    {
        IsDialInBypassEnabled = true
    }
};

await graphClient.Me.OnlineMeetings["{onlineMeeting-id}"]
    .Request()
    .UpdateAsync(onlineMeeting);

```