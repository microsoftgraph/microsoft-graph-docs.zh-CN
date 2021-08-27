---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8909eb360fd37d2d23767ed03859ef7d81e6dc29a207a1ff5057c37f197fe97c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332947"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chatMessage = new ChatMessage
{
    Body = new ItemBody
    {
        ContentType = BodyType.Html,
        Content = "Hello World"
    }
};

await graphClient.Teams["{team-id}"].Channels["{channel-id}"].Messages["{chatMessage-id}"].Replies
    .Request()
    .AddAsync(chatMessage);

```