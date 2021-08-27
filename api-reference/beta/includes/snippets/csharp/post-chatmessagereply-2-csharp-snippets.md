---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 10c3a4b65f7cd00e6b0afb22aef9cfddaf15c8abcc9ceca782404cdb6b45380f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332949"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chatMessage = new ChatMessage
{
    CreatedDateTime = DateTimeOffset.Parse("2019-02-04T19:58:15.511Z"),
    From = new ChatMessageFromIdentitySet
    {
        User = new Identity
        {
            Id = "8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca",
            DisplayName = "John Doe"
        }
    },
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