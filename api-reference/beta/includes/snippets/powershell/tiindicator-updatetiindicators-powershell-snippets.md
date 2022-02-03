---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 199ea7d66675ba19d940d2a113a30c1c4d03903b
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62341896"
---
```powershell

Import-Module Microsoft.Graph.Security

$params = @{
    Value = @(
        @{
            Id = "c6fb948b-89c5-3bba-a2cd-a9d9a1e430e4"
            AdditionalInformation = "mytest"
        }
        @{
            Id = "e58c072b-c9bb-a5c4-34ce-eb69af44fb1e"
            AdditionalInformation = "test again"
        }
    )
}

Update-MgSecurityTiIndicatorMultiple -BodyParameter $params

```