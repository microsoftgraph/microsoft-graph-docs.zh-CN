---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 119ab43f51709cc110f28dee9391bac4b21b0e6a
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208452"
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
            Id = "id-value",
            DisplayName = "Joh Doe",
            UserIdentityType = TeamworkUserIdentityType.AadUser
        }
    },
    Body = new ItemBody
    {
        ContentType = BodyType.Html,
        Content = "Hello World"
    }
};

await graphClient.Teams["{team-id}"].Channels["{channel-id}"].Messages
    .Request()
    .AddAsync(chatMessage);

```