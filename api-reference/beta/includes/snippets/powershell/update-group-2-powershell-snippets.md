---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1267719a42123dc6830b973c5ac55b3d8eafb142
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62133537"
---
```powershell

Import-Module Microsoft.Graph.Groups

$params = @{
    AssignedLabels = @(
        @{
            LabelId = "45cd0c48-c540-4358-ad79-a3658cdc5b88"
        }
    )
}

Update-MgGroup -GroupId $groupId -BodyParameter $params

```