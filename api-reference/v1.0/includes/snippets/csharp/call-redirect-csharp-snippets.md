---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e04919f66502bdd927aa720569d712e1d90887c34c57c6bfcc75700112f09fec
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332811"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var targets = new List<InvitationParticipantInfo>()
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

var callbackUri = "https://bot.contoso.com/api/calls/24701998-1a73-4d42-8085-bf46ed0ae039";

await graphClient.Communications.Calls["{call-id}"]
    .Redirect(targets,null,callbackUri)
    .Request()
    .PostAsync();

```