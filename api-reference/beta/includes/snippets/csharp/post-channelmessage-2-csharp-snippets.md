---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7d636dc9664081b1add718599b3ca34efb2ef77b47fc71640f67b7b0c6ed6e03
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277360"
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