---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6188c38d72b41f0ecda9d413517cfd14fb966611
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963034"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var participants = new List<InvitationParticipantInfo>()
{
    new InvitationParticipantInfo
    {
        Identity = new IdentitySet
        {
            AdditionalData = new Dictionary<string, object>()
            {
                {"phone", "{\"@odata.type\":\"#microsoft.graph.identity\",\"id\":\"+12345678901\"}"}
            }
        }
    }
};

var clientContext = "f2fa86af-3c51-4bc2-8fc0-475452d9764f";

await graphClient.Communications.Calls["{call-id}"].Participants
    .Invite(participants,clientContext)
    .Request()
    .PostAsync();

```