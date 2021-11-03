---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e22b4a9a22b6541380a212cc2b80e9b24d5271f
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60688936"
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
        {"user@odata.bind", "https://graph.microsoft.com/beta/users/jacob@contoso.com"}
    }
};

await graphClient.Chats["{chat-id}"].Members
    .Request()
    .AddAsync(conversationMember);

```