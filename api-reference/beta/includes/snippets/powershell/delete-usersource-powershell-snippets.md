---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 05ccfaf10658577fda22b8a9054f0ae381721a80
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62123730"
---
```powershell

Import-Module Microsoft.Graph.Compliance

Remove-MgComplianceEdiscoveryCaseCustodianUserSource -CaseId $caseId -CustodianId $custodianId -UserSourceId $userSourceId

```