---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cc8dcd4ed28ef3375973a97cba12f2f1d4c8e50d
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62347368"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
    CallbackUri = "https://bot.contoso.com/api/calls"
    AcceptedModalities = @(
        "audio"
    )
    MediaConfig = @{
        "@odata.type" = "#microsoft.graph.appHostedMediaConfig"
        Blob = "<Media Session Configuration Blob>"
    }
}

Invoke-MgAnswerCommunicationCall -CallId $callId -BodyParameter $params

```