---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 12470bc3f622d2335c23e9da467cd9440601b36e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62133838"
---
```powershell

Import-Module Microsoft.Graph.Compliance

Get-MgComplianceEdiscoveryCaseCustodian -CaseId $caseId -CustodianId $custodianId

```