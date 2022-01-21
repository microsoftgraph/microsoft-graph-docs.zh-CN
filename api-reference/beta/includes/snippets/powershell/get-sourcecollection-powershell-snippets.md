---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eca91e219f7aaa1574a3e5d62d907fb11513ca36
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62133810"
---
```powershell

Import-Module Microsoft.Graph.Compliance

Get-MgComplianceEdiscoveryCaseSourceCollection -CaseId $caseId -SourceCollectionId $sourceCollectionId -ExpandProperty "addToReviewSetOperation,custodianSources,lastEstimateStatisticsOperation" 

```