---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5f069885e8b9a1aadbc14b0fc51c3baed372f522
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62344373"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
    TransferTarget = @{
        EndpointType = "default"
        Identity = @{
            Phone = @{
                "@odata.type" = "#microsoft.graph.identity"
                Id = "+12345678901"
            }
        }
        LanguageId = "languageId-value"
        Region = "region-value"
    }
    ClientContext = "9e90d1c1-f61e-43e7-9f75-d420159aae08"
}

Move-MgCommunicationCall -CallId $callId -BodyParameter $params

```