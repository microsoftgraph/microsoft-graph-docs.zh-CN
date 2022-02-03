---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5cac3d2ce67064554bccad59335c5b052bd3684a
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62344372"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
    TransferTarget = @{
        "@odata.type" = "#microsoft.graph.invitationParticipantInfo"
        EndpointType = "default"
        Identity = @{
            "@odata.type" = "#microsoft.graph.identitySet"
            Phone = @{
                "@odata.type" = "#microsoft.graph.identity"
                Id = "+12345678901"
            }
        }
        LanguageId = "en-us"
        Region = "amer"
        ReplacesCallId = "e5d39592-99bd-4db8-bca8-30fb894ec51d"
    }
    ClientContext = "9e90d1c1-f61e-43e7-9f75-d420159aae08"
}

Move-MgCommunicationCall -CallId $callId -BodyParameter $params

```