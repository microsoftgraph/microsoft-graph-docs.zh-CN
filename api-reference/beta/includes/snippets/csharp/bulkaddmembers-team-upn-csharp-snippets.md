---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6cb782664bd5ef8ef07424b7a959cf38abcf9f1e
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60689421"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var values = new List<ConversationMember>()
{
    new AadUserConversationMember
    {
        Roles = new List<String>()
        {
        },
        AdditionalData = new Dictionary<string, object>()
        {
            {"user@odata.bind", "https://graph.microsoft.com/beta/users('jacob@contoso.com')"}
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
            {"user@odata.bind", "https://graph.microsoft.com/beta/users('alex@contoso.com')"}
        }
    }
};

await graphClient.Teams["{team-id}"].Members
    .Add(values)
    .Request()
    .PostAsync();

```