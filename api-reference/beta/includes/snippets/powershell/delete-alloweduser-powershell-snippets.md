---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d0b9bc07072e5e506a934f7762af6ecc045be759
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437960"
---
```powershell

Import-Module Microsoft.Graph.Devices.CloudPrint

Remove-MgPrintPrinterShareAllowedUserByRef -PrinterShareId $printerShareId -UserId $userId

```