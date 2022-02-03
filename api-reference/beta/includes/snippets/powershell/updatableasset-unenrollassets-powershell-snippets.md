---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 666a3becfe6965cf914c3effef6764471047d943
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62343784"
---
```powershell

Import-Module Microsoft.Graph.WindowsUpdates

$params = @{
    UpdateCategory = "String"
    Assets = @(
        @{
            "@odata.type" = "#microsoft.graph.windowsUpdates.azureADDevice"
            Id = "String (identifier)"
        }
    )
}

Invoke-MgUnenrollWindowsUpdatesUpdatableAsset -BodyParameter $params

```