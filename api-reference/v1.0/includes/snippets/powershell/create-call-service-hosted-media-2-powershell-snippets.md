---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e962c25ff35a37a548bac1043ffa04f30ba91306
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62136575"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
    "@odata.type" = "#microsoft.graph.call"
    CallbackUri = "https://bot.contoso.com/callback"
    Source = @{
        "@odata.type" = "#microsoft.graph.participantInfo"
        Identity = @{
            "@odata.type" = "#microsoft.graph.identitySet"
            ApplicationInstance = @{
                "@odata.type" = "#microsoft.graph.identity"
                DisplayName = "Calling Bot"
                Id = "3d913abb-aec0-4964-8fa6-3c6850c4f278"
            }
        }
        CountryCode = $null
        EndpointType = $null
        Region = $null
        LanguageId = $null
    }
    Targets = @(
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
    RequestedModalities = @(
        "audio"
    )
    MediaConfig = @{
        "@odata.type" = "#microsoft.graph.serviceHostedMediaConfig"
    }
    TenantId = "aa67bd4c-8475-432d-bd41-39f255720e0a"
}

New-MgCommunicationCall -BodyParameter $params

```