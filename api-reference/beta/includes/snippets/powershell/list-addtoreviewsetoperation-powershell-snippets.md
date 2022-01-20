---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 724a9eda74a62e2e2227eda2b4cdf29deaa39a8b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62127951"
---
```powershell

Import-Module Microsoft.Graph.Compliance

Get-MgComplianceEdiscoveryCaseSourceCollectionAddToReviewSetOperation -CaseId $caseId -SourceCollectionId $sourceCollectionId

```