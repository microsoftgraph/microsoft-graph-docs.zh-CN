---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b77c31fea5004cd2b2c29ea27c7aba004d032809
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62344376"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
    TransferTarget = @{
        "@odata.type" = "#microsoft.graph.invitationParticipantInfo"
        EndpointType = "default"
        Identity = @{
            "@odata.type" = "#microsoft.graph.identitySet"
            User = @{
                "@odata.type" = "#microsoft.graph.identity"
                Id = "550fae72-d251-43ec-868c-373732c2704f"
                DisplayName = "Heidi Steen"
            }
        }
        ReplacesCallId = "e5d39592-99bd-4db8-bca8-30fb894ec51d"
    }
}

Move-MgCommunicationCall -CallId $callId -BodyParameter $params

```