---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ad8a9a34c30f10e7f8c65ecffb00c57bcacce68
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62342484"
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

Add-MgWindowsUpdatesUpdatableAssetMember -UpdatableAssetId $updatableAssetId -BodyParameter $params

```