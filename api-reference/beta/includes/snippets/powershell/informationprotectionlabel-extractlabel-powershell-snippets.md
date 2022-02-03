---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 83be870630a29998301714fb948e39344bfc570c
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349187"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    ContentInfo = @{
        "@odata.type" = "#microsoft.graph.contentInfo"
        "Format@odata.type" = "#microsoft.graph.contentFormat"
        Format = "default"
        Identifier = $null
        "State@odata.type" = "#microsoft.graph.contentState"
        State = "rest"
        "Metadata@odata.type" = "#Collection(microsoft.graph.keyValuePair)"
        Metadata = @(
            @{
                "@odata.type" = "#microsoft.graph.keyValuePair"
                Name = "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Enabled"
                Value = "True"
            }
            @{
                "@odata.type" = "#microsoft.graph.keyValuePair"
                Name = "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Method"
                Value = "Standard"
            }
            @{
                "@odata.type" = "#microsoft.graph.keyValuePair"
                Name = "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SetDate"
                Value = "1/1/0001 12:00:00 AM"
            }
            @{
                "@odata.type" = "#microsoft.graph.keyValuePair"
                Name = "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SiteId"
                Value = "cfa4cf1d-a337-4481-aa99-19d8f3d63f7c"
            }
            @{
                "@odata.type" = "#microsoft.graph.keyValuePair"
                Name = "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Name"
                Value = "Top Secret"
            }
            @{
                "@odata.type" = "#microsoft.graph.keyValuePair"
                Name = "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ContentBits"
                Value = "0"
            }
            @{
                "@odata.type" = "#microsoft.graph.keyValuePair"
                Name = "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ActionId"
                Value = "00000000-0000-0000-0000-000000000000"
            }
        )
    }
}

Invoke-MgExtractInformationProtectionPolicyLabel -BodyParameter $params

```