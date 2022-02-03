---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6668faa1df11361bae1aba2719efc7f0fb20ff66
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62342495"
---
```powershell

Import-Module Microsoft.Graph.WindowsUpdates

$params = @{
    UpdateCategory = "feature"
    MemberEntityType = "#microsoft.graph.windowsUpdates.azureADDevice"
    Ids = @(
        "String"
        "String"
        "String"
    )
}

Invoke-MgEnrollWindowsUpdatesUpdatableAssetById -BodyParameter $params

```