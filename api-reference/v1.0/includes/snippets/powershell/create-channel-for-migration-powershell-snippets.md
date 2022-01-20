---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c0e618d067eb68a33cbb0b8977d6357cf4207784
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62101581"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    "@microsoft.graph.channelCreationMode" = "migration"
    DisplayName = "Import_150958_99z"
    Description = "Import_150958_99z"
    CreatedDateTime = [System.DateTime]::Parse("2020-03-14T11:22:17.067Z")
}

New-MgTeamChannel -TeamId $teamId -BodyParameter $params

```