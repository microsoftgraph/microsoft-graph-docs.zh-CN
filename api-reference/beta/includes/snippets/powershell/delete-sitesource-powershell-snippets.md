---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 79f7897b5c99df1bfda586d107145d0b0ceb3538
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62120839"
---
```powershell

Import-Module Microsoft.Graph.Compliance

Remove-MgComplianceEdiscoveryCaseCustodianSiteSource -CaseId $caseId -CustodianId $custodianId -SiteSourceId $siteSourceId

```