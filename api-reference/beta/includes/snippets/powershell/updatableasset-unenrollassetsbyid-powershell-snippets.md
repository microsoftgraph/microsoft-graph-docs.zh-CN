---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 83115c035a4c578b1e4373a6fa323a8ee158d0cb
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62348116"
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

Invoke-MgUnenrollWindowsUpdatesUpdatableAssetById -BodyParameter $params

```