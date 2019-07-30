---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 391c26b56023314d79c0351051ca2097fc9e697c
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35933817"
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
    .Redirect(targets,targetDisposition,timeout,maskCallee,maskCaller,callbackUri)
    .Request()
    .PostAsync();

```