---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 85f511fad5711240e2384765e21f891eace33d88
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62104582"
---
```powershell

Import-Module Microsoft.Graph.Devices.CloudPrint

$params = @{
    DisplayName = "PrinterShare Name"
    "Printer@odata.bind" = "https://graph.microsoft.com/v1.0/print/printers/{printerId}"
    AllowAllUsers = $false
}

Update-MgPrintShare -PrinterShareId $printerShareId -BodyParameter $params

```