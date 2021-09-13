---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1705592ddc24740e9d48e584b796763ebbafacf305f6cbf9ad8acb90e5a96001
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902993"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversationMember = new AadUserConversationMember
{
    Roles = new List<String>()
    {
    },
    AdditionalData = new Dictionary<string, object>()
    {
        {"user@odata.bind", "https://graph.microsoft.com/v1.0/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5"}
    }
};

await graphClient.Teams["{team-id}"].Channels["{channel-id}"].Members
    .Request()
    .AddAsync(conversationMember);

```