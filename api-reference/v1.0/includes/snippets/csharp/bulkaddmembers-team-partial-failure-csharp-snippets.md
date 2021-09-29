---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 907da988bb2dcc5b01ecad208af8038b55137b09
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996731"
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
            {"user@odata.bind", "https://graph.microsoft.com/v1.0/users('18a80140-b0fb-4489-b360-2f6efaf225a0')"}
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
            {"user@odata.bind", "https://graph.microsoft.com/v1.0/users('86503198-b81b-43fe-81ee-ad45b8848ac9')"}
        }
    }
};

await graphClient.Teams["{team-id}"].Members
    .Add(values)
    .Request()
    .PostAsync();

```