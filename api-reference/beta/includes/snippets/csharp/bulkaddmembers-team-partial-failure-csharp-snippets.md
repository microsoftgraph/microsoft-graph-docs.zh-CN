---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 15ad9cbc22bb2300312e3e6f95ddc0fffacf8ad4b4cba4f30e06bb1f2b5af1a2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158300"
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
            {"user@odata.bind", "https://graph.microsoft.com/beta/users('18a80140-b0fb-4489-b360-2f6efaf225a0')"}
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
            {"user@odata.bind", "https://graph.microsoft.com/beta/users('86503198-b81b-43fe-81ee-ad45b8848ac9')"}
        }
    }
};

await graphClient.Teams["{team-id}"].Members
    .Add(values)
    .Request()
    .PostAsync();

```