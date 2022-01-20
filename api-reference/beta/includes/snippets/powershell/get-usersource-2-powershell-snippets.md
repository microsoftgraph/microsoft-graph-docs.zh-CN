---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3f48afd41245eeffc03441bfbbf3264266f4a589
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62103266"
---
```powershell

Import-Module Microsoft.Graph.Compliance

Get-MgComplianceEdiscoveryCaseCustodianUserSource -CaseId $caseId -CustodianId $custodianId -UserSourceId $userSourceId

```