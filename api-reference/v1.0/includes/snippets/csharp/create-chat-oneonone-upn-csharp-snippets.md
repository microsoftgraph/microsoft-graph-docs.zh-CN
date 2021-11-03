---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7187d860425ea2abeadb65ae4e23caafa44e36f2
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696887"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chat = new Chat
{
    ChatType = ChatType.OneOnOne,
    Members = new ChatMembersCollectionPage()
    {
        new AadUserConversationMember
        {
            Roles = new List<String>()
            {
                "owner"
            },
            AdditionalData = new Dictionary<string, object>()
            {
                {"user@odata.bind", "https://graph.microsoft.com/v1.0/users('jacob@contoso.com')"}
            }
        },
        new AadUserConversationMember
        {
            Roles = new List<String>()
            {
                "owner"
            },
            AdditionalData = new Dictionary<string, object>()
            {
                {"user@odata.bind", "https://graph.microsoft.com/v1.0/users('alex@contoso.com')"}
            }
        }
    }
};

await graphClient.Chats
    .Request()
    .AddAsync(chat);

```