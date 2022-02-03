---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a9fcce42eaaeb312de2c0d4638c2ea54158eb720
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62341898"
---
```powershell

Import-Module Microsoft.Graph.Security

$params = @{
    Value = @(
        "id-value1"
        "id-value2"
    )
}

Remove-MgSecurityTiIndicatorMultiple -BodyParameter $params

```