---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3f6b019ce2d0c2dae4d72337f9880d562e0254ba
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62341375"
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
                TenantId = "72f988bf-86f1-41af-91ab-2d7cd011db47"
                DisplayName = "Heidi Steen"
            }
        }
        LanguageId = "en-us"
        Region = "amer"
        ReplacesCallId = "e5d39592-99bd-4db8-bca8-30fb894ec51d"
    }
}

Move-MgCommunicationCall -CallId $callId -BodyParameter $params

```