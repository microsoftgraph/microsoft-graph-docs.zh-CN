---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bfa83cd41d37452e7405226045f0c9b02bd5eaa0
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62344374"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
    TransferTarget = @{
        EndpointType = "default"
        Identity = @{
            User = @{
                Id = "550fae72-d251-43ec-868c-373732c2704f"
                DisplayName = "Heidi Steen"
            }
        }
    }
}

Move-MgCommunicationCall -CallId $callId -BodyParameter $params

```