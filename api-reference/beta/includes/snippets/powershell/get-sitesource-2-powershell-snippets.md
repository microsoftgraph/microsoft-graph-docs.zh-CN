---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1dcf6047abc02cc6e254cf69ca6f69bb6d527b2a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62133824"
---
```powershell

Import-Module Microsoft.Graph.Compliance

Get-MgComplianceEdiscoveryCaseCustodianSiteSource -CaseId $caseId -CustodianId $custodianId -SiteSourceId $siteSourceId

```