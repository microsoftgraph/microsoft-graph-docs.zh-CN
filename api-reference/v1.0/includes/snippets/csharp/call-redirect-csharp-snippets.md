---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c90875bfd613217128161738014f47bd390e49c0
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871105"
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
    .Redirect(targets,null,callbackUri)
    .Request()
    .PostAsync();

```