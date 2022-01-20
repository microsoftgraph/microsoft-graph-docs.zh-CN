---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 42822a6c0bb36ed75f82f3b3fc49d18ab34afe14
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62134454"
---
```powershell

Import-Module Microsoft.Graph.Devices.CloudPrint

$params = @{
    "@odata.id" = "https://graph.microsoft.com/v1.0/groups/{groupId}"
}

New-MgPrintShareAllowedGroupByRef -PrinterShareId $printerShareId -BodyParameter $params

```