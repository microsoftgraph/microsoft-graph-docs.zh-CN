---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c9b07ee0ad5f5fc1784af4fda60dc5da7a15270a
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522110"
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
        {"user@odata.bind", "https://graph.microsoft.com/v1.0/users('8b081ef6-4792-4def-b2c9-c363a1bf41d5')"}
    }
};

await graphClient.Teams["ece6f0a1-7ca4-498b-be79-edf6c8fc4d82"].Channels["19:56eb04e133944cf69e603c5dac2d292e@thread.skype"].Members
    .Request()
    .AddAsync(conversationMember);

```