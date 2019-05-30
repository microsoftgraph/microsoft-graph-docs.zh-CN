---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6baa80e9ed4ca4ab9c118d20e276fd554a744cd9
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/29/2019
ms.locfileid: "34546617"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var targets = new List<InvitationParticipantInfo>()
{
    new InvitationParticipantInfo
    {
        EndpointType = EndpointType.Default,
        Identity = new IdentitySet
        {
            User = new Identity
            {
                Id = "550fae72-d251-43ec-868c-373732c2704f",
                TenantId = "72f988bf-86f1-41af-91ab-2d7cd011db47",
                DisplayName = "Heidi Steen"
            }
        },
        LanguageId = "en-US",
        Region = "westus"
    }
};

var targetDisposition = CallDisposition.Default;

var timeout = 99;

var maskCallee = false;

var maskCaller = false;

await graphClient.App.Calls["{id}"]
    .Redirect(targets,targetDisposition,timeout,maskCallee,maskCaller)
    .Request()
    .PostAsync();

```