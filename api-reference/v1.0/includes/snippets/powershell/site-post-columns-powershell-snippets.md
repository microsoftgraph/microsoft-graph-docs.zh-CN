---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3342d8ba84495b01df03733ff1dc156ded365aa8
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62134300"
---
```powershell

Import-Module Microsoft.Graph.Sites

$params = @{
    Description = "test"
    EnforceUniqueValues = $false
    Hidden = $false
    Indexed = $false
    Name = "Title"
    Text = @{
        AllowMultipleLines = $false
        AppendChangesToExistingText = $false
        LinesForEditing = 0
        MaxLength = 255
    }
}

New-MgSiteColumn -SiteId $siteId -BodyParameter $params

```