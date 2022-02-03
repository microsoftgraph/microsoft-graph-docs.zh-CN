---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1942670c6170a1369ffe568fd16ecef94ee4de30
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62346213"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
    CustomPrompt = @{
        "@odata.type" = "#microsoft.graph.mediaPrompt"
        MediaInfo = @{
            "@odata.type" = "#microsoft.graph.mediaInfo"
            Uri = "https://bot.contoso.com/onHold.wav"
        }
    }
    ClientContext = "d45324c1-fcb5-430a-902c-f20af696537c"
}

Start-MgCommunicationCallParticipantHoldMusic -CallId $callId -ParticipantId $participantId -BodyParameter $params

```