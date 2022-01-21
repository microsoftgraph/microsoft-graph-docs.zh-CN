---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f25da6e2b1e5cadd6be9e8bc9aa3ecbc4eec42b5
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62103308"
---
```powershell

Import-Module Microsoft.Graph.Compliance

Get-MgComplianceEdiscoveryCaseReviewSet -CaseId $caseId -ReviewSetId $reviewSetId

```