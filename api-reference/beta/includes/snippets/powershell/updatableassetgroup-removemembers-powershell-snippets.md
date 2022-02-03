---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3f4a5ecf89b2e75c74e11d6c1ebfa6a4d6b38e02
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62340055"
---
```powershell

Import-Module Microsoft.Graph.WindowsUpdates

$params = @{
    Assets = @(
        @{
            "@odata.type" = "#microsoft.graph.windowsUpdates.azureADDevice"
            Id = "String (identifier)"
        }
    )
}

Remove-MgWindowsUpdatesUpdatableAssetMember -UpdatableAssetId $updatableAssetId -BodyParameter $params

```