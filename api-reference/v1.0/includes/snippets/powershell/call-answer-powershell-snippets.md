---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ce65f5b9e2eba4598db00b77f1c61dc766e802f7
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62347367"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
    CallbackUri = "callbackUri-value"
    MediaConfig = @{
        "@odata.type" = "#microsoft.graph.appHostedMediaConfig"
        Blob = "<Media Session Configuration Blob>"
    }
    AcceptedModalities = @(
        "audio"
    )
    ParticipantCapacity = 200
}

Invoke-MgAnswerCommunicationCall -CallId $callId -BodyParameter $params

```