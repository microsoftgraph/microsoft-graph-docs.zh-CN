---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d79789c0ef1b45628b2815129f8df33a0d3ce7ae
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62091974"
---
```powershell

Import-Module Microsoft.Graph.Devices.CloudPrint

$params = @{
    Name = "PrinterName"
    Location = @{
        Latitude = 1.1
        Longitude = 2.2
        AltitudeInMeters = 3
    }
}

Update-MgPrintPrinter -PrinterId $printerId -BodyParameter $params

```