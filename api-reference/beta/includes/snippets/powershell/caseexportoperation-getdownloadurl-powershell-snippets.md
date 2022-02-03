---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2a1d320e8ac2037c54adfd40147961df6cbf8ff3
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62346884"
---
```powershell

Import-Module Microsoft.Graph.Compliance

Get-MgComplianceEdiscoveryCaseOperationMicrosoftGraphEdiscoveryCaseExportOperationDownloadUrl -CaseId $caseId -CaseOperationId $caseOperationId

```