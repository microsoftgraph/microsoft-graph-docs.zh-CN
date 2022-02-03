---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b897d11c11020cc1ae2da3bbd65aa83d0ca06fe8
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62341376"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
    TransferTarget = @{
        EndpointType = "default"
        Identity = @{
            User = @{
                Id = "550fae72-d251-43ec-868c-373732c2704f"
                TenantId = "72f988bf-86f1-41af-91ab-2d7cd011db47"
                DisplayName = "Heidi Steen"
            }
        }
    }
    Transferee = @{
        Identity = @{
            User = @{
                Id = "751f6800-3180-414d-bd94-333364659951"
                TenantId = "72f988bf-86f1-41af-91ab-2d7cd011db47"
            }
        }
        ParticipantId = "909c6581-5130-43e9-88f3-fcb3582cde37"
    }
    LanguageId = "languageId-value"
    Region = "region-value"
}

Move-MgCommunicationCall -CallId $callId -BodyParameter $params

```