---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f9a7dddd82a331a54dc1f86a727b0770a2c91ba1
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62134496"
---
```powershell

Import-Module Microsoft.Graph.Devices.CloudPrint

$params = @{
    DisplayName = "ShareName"
    AllowAllUsers = $false
    "Printer@odata.bind" = "https://graph.microsoft.com/v1.0/print/printers/{printerId}"
}

New-MgPrintShare -BodyParameter $params

```