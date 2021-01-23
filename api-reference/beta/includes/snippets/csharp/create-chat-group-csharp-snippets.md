---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c8f47dc0fe7a6dc95439344e416deadc22cae3e0
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945650"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chat = new Chat
{
    ChatType = ChatType.Group,
    Topic = "Group chat title",
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
                {"user@odata.bind", "https://graph.microsoft.com/beta/users('8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca')"}
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
                {"user@odata.bind", "https://graph.microsoft.com/beta/users('82fe7758-5bb3-4f0d-a43f-e555fd399c6f')"}
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
                {"user@odata.bind", "https://graph.microsoft.com/beta/users('3626a173-f2bc-4883-bcf7-01514c3bfb82')"}
            }
        }
    }
};

await graphClient.Chats
    .Request()
    .AddAsync(chat);

```