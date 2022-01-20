---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ef05dd1f542a775a2e5aacae0423ddb5f4a67d7
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62100164"
---
```powershell

Import-Module Microsoft.Graph.Compliance

Get-MgComplianceEdiscoveryCaseReviewSetQuery -CaseId $caseId -ReviewSetId $reviewSetId

```