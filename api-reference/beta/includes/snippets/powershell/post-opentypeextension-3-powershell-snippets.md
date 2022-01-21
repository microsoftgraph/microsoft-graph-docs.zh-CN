---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 03ddde4278b7cfaaba8a77c039101b88d8a9a451
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62130930"
---
```powershell

Import-Module Microsoft.Graph.Calendar

$params = @{
    "@odata.type" = "microsoft.graph.openTypeExtension"
    ExtensionName = "Com.Contoso.Deal"
    CompanyName = "Alpine Skis"
    DealValue = 
    ExpirationDate = "2015-07-03T13:04:00.000Z"
}

New-MgGroupEventExtension -GroupId $groupId -EventId $eventId -BodyParameter $params

```