---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d1c8c08cbfd7764e07766cbde03d94c306acadb48de0d9802f8c411e65ca4d7f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218742"
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