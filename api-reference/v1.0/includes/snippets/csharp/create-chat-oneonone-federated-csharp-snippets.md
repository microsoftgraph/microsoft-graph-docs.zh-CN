---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8d1a669b2e8e99a88162d24679bac5f47b160811
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437855"
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
                {"user@odata.bind", "https://graph.microsoft.com/v1.0/users('8b081ef6-4792-4def-b2c9-c363a1bf41d5')"}
            }
        },
        new AadUserConversationMember
        {
            Roles = new List<String>()
            {
                "owner"
            },
            TenantId = "4dc1fe35-8ac6-4f0d-904a-7ebcd364bea1",
            AdditionalData = new Dictionary<string, object>()
            {
                {"user@odata.bind", "https://graph.microsoft.com/v1.0/users('82af01c5-f7cc-4a2e-a728-3a5df21afd9d')"}
            }
        }
    }
};

await graphClient.Chats
    .Request()
    .AddAsync(chat);

```