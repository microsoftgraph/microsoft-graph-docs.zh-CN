---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ca1f6b891d1aee737778a5ba2229f13f05ede44
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66442906"
---
```powershell

Import-Module Microsoft.Graph.Devices.CloudPrint

Remove-MgPrintShareAllowedUserByRef -PrinterShareId $printerShareId -UserId $userId

```