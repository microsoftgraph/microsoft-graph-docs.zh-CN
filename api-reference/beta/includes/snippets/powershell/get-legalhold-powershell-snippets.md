---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4298f1b490da2b82276ca5347422dbf56ebf475e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62123933"
---
```powershell

Import-Module Microsoft.Graph.Compliance

Get-MgComplianceEdiscoveryCaseLegalHold -CaseId $caseId -LegalHoldId $legalHoldId

```