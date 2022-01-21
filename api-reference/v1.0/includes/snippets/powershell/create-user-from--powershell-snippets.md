---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1a73058fb9e0bb029b155c88ea17f3a2c852cd50
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62135721"
---
```powershell

Import-Module Microsoft.Graph.Devices.CloudPrint

$params = @{
    "@odata.id" = "https://graph.microsoft.com/v1.0/users/{userId}"
}

New-MgPrintShareAllowedUserByRef -PrinterShareId $printerShareId -BodyParameter $params

```