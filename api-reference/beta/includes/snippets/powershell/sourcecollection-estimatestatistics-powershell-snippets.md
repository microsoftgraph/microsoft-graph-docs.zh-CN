---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3eac903021b1539f51dda11322b1fca80d158f7a
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62340255"
---
```powershell

Import-Module Microsoft.Graph.Compliance

Invoke-MgEstimateComplianceEdiscoveryCaseSourceCollectionStatistics -CaseId $caseId -SourceCollectionId $sourceCollectionId

```