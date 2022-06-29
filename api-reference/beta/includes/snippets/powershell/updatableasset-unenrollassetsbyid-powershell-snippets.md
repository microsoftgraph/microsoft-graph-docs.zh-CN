---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a4a483657f9e09f17ce68e26b230719fb9a41ed6
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66502697"
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

Invoke-MgGraphWindowsUpdatesUpdatableAsset -BodyParameter $params

```