---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6a5e49d3092198931b174c2a4ab205af4acadd26
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/13/2019
ms.locfileid: "38302869"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var targets = new List<InvitationParticipantInfo>()
{
    new InvitationParticipantInfo
    {
        Identity = new IdentitySet
        {
            Application = new Identity
            {
                DisplayName = "test bot 2",
                Id = "22bfd41f-550e-477d-8789-f6f7bd2a5e8b"
            }
        }
    }
};

var callbackUri = "https://bot.contoso.com/api/calls/24701998-1a73-4d42-8085-bf46ed0ae039";

await graphClient.Communications.Calls["491f0b00-ffff-4bc9-a43e-b226498ec22a"]
    .Redirect(targets,null,null,null,null,callbackUri)
    .Request()
    .PostAsync();

```