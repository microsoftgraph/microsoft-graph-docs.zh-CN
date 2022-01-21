---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: edb961c5a1328e527412dfdc3bdd03b2a0b14f31
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62135904"
---
```powershell

Import-Module Microsoft.Graph.Calendar

$params = @{
    "@odata.type" = "microsoft.graph.room"
    Nickname = "Conf Room"
    Building = "1"
    Label = "100"
    Capacity = 
    IsWheelChairAccessible = $false
}

Update-MgPlace -PlaceId $placeId -BodyParameter $params

```