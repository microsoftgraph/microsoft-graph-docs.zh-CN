---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e6b91644190860fc828af367599b18118b3fcabb
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62347296"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
    Targets = @(
        @{
            "@odata.type" = "#microsoft.graph.invitationParticipantInfo"
            Identity = @{
                "@odata.type" = "#microsoft.graph.identitySet"
                Phone = @{
                    "@odata.type" = "#microsoft.graph.identity"
                    Id = "+12345678901"
                }
            }
        }
    )
    CallbackUri = "https://bot.contoso.com/api/calls/24701998-1a73-4d42-8085-bf46ed0ae039"
}

Invoke-MgRedirectCommunicationCall -CallId $callId -BodyParameter $params

```