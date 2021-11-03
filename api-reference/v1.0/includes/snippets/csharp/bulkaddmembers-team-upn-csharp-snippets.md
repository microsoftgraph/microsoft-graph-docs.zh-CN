---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ee7211c3df5188de06916e26e8211b8ed1d4313d
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60688405"
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
};

await graphClient.Teams["{team-id}"].Members
    .Add(values)
    .Request()
    .PostAsync();

```