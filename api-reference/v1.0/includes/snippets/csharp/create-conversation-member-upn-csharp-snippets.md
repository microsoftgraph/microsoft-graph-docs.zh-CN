---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ad5b84994981189a0baff9eed3d66b3d6fe10472
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696542"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversationMember = new AadUserConversationMember
{
    VisibleHistoryStartDateTime = DateTimeOffset.Parse("2019-04-18T23:51:43.255Z"),
    Roles = new List<String>()
    {
        "owner"
    },
    AdditionalData = new Dictionary<string, object>()
    {
        {"user@odata.bind", "https://graph.microsoft.com/v1.0/users/jacob@contoso.com"}
    }
};

await graphClient.Chats["{chat-id}"].Members
    .Request()
    .AddAsync(conversationMember);

```