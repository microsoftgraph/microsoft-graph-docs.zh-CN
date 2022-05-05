---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c66abc63f7f5a6e4c50b0fdc776f6375efa4b0c1
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65220264"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
    "@odata.type" = "#microsoft.graph.call"
    CallbackUri = "https://bot.contoso.com/callback"
    Targets = @(
        @{
            "@odata.type" = "#microsoft.graph.invitationParticipantInfo"
            Identity = @{
                "@odata.type" = "#microsoft.graph.identitySet"
                User = @{
                    "@odata.type" = "#microsoft.graph.identity"
                    DisplayName = "John"
                    Id = "112f7296-5fa4-42ca-bae8-6a692b15d4b8"
                }
            }
        }
    )
    RequestedModalities = @(
        "audio"
    )
    CallOptions = @{
        "@odata.type" = "#microsoft.graph.outgoingCallOptions"
        IsContentSharingNotificationEnabled = $true
    }
    MediaConfig = @{
        "@odata.type" = "#microsoft.graph.serviceHostedMediaConfig"
    }
}

New-MgCommunicationCall -BodyParameter $params

```