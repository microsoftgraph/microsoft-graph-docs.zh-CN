---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b7b12d5af8d3c1391dac0d629c715837892bcf27
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62135693"
---
```powershell

Import-Module Microsoft.Graph.Devices.CloudPrint

Get-MgPrintPrinterTaskTrigger -PrinterId $printerId -PrintTaskTriggerId $printTaskTriggerId

```