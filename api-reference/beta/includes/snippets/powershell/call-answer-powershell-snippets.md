---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5369ce02d46ace9f8e09de4708a29fc0047b296c
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65220301"
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
    CallOptions = @{
        "@odata.type" = "#microsoft.graph.incomingCallOptions"
        IsContentSharingNotificationEnabled = $true
    }
    ParticipantCapacity = 200
}

Invoke-MgAnswerCommunicationCall -CallId $callId -BodyParameter $params

```