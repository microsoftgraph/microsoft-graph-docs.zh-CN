---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 10fa0d118d46086d92e8863b08f11bbad69087d2
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62338979"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
    Participants = @(
        @{
            "@odata.type" = "#microsoft.graph.invitationParticipantInfo"
            ReplacesCallId = "a7ebfb2d-871e-419c-87af-27290b22e8db"
            Identity = @{
                "@odata.type" = "#microsoft.graph.identitySet"
                User = @{
                    "@odata.type" = "#microsoft.graph.identity"
                    Id = "7e1b4346-85a6-4bdd-abe3-d11c5d420efe"
                    DisplayName = "string"
                }
            }
        }
    )
    ClientContext = "f2fa86af-3c51-4bc2-8fc0-475452d9764f"
}

Invoke-MgInviteCommunicationCallParticipant -CallId $callId -BodyParameter $params

```