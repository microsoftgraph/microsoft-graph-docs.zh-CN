---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 39ef1bf2054dfeab8f484a817271775685b9d7a8
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62124493"
---
```powershell

Import-Module Microsoft.Graph.Devices.CloudPrint

Get-MgPrintTaskDefinitionTask -PrintTaskDefinitionId $printTaskDefinitionId -PrintTaskId $printTaskId

```