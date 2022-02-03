---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9fc06ff023662aa21943fb93ad30d60ae281c3a4
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62348129"
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

Invoke-MgEnrollWindowsUpdatesUpdatableAsset -BodyParameter $params

```