---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d7662099923f7c283e3c88e10d697b5cca3039a3
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62118381"
---
```powershell

Import-Module Microsoft.Graph.Devices.CloudPrint

$params = @{
    DisplayName = "ShareName"
    AllowAllUsers = $true
    "Printer@odata.bind" = "https://graph.microsoft.com/beta/print/printers/{id}"
}

Update-MgPrintShare -PrinterShareId $printerShareId -BodyParameter $params

```