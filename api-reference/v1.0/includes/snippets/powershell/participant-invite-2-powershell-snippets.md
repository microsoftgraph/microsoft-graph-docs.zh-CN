---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8667343c77cf9050ff140cb78cffb5a5fcdcfe68
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62338981"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
    Participants = @(
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
    ClientContext = "f2fa86af-3c51-4bc2-8fc0-475452d9764f"
}

Invoke-MgInviteCommunicationCallParticipant -CallId $callId -BodyParameter $params

```