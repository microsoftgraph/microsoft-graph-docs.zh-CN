---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 12fcf9689c3761e9ebed698586d64e7728c9ef48
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62123842"
---
```powershell

Import-Module Microsoft.Graph.Compliance

Get-MgComplianceEdiscoveryCaseReviewSetQuery -CaseId $caseId -ReviewSetId $reviewSetId -ReviewSetQueryId $reviewSetQueryId

```