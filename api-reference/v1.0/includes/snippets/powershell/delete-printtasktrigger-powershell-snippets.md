---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: edded01df423ebc9580686c9a813f4ef11abfd1e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62088319"
---
```powershell

Import-Module Microsoft.Graph.Devices.CloudPrint

Remove-MgPrintPrinterTaskTrigger -PrinterId $printerId -PrintTaskTriggerId $printTaskTriggerId

```