---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6fbb1f96e217ee900c0f1ee84174c0bdb86428d4
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60689141"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversationMember = new AadUserConversationMember
{
    Roles = new List<String>()
    {
        "owner"
    },
    AdditionalData = new Dictionary<string, object>()
    {
        {"user@odata.bind", "https://graph.microsoft.com/beta/users('jacob@contoso.com')"}
    }
};

await graphClient.Teams["{team-id}"].Channels["{channel-id}"].Members
    .Request()
    .AddAsync(conversationMember);

```