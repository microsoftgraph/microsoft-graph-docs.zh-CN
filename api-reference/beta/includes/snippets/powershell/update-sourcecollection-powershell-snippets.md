---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 77bde6a5af00c4a64fef72e7c40ab2ef340cc799
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62090358"
---
```powershell

Import-Module Microsoft.Graph.Compliance

$params = @{
    DisplayName = "Quarterly Financials search"
}

Update-MgComplianceEdiscoveryCaseSourceCollection -CaseId $caseId -SourceCollectionId $sourceCollectionId -BodyParameter $params

```