---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7145d5e52c486e1a896d08450ff9c257d614341b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62133768"
---
```powershell

Import-Module Microsoft.Graph.Compliance

$params = @{
    "@odata.id" = "https://canary.graph.microsoft.com/testprodbetancsdsaslist/compliance/ediscovery/cases/06d52284-ed81-49b8-904a-b863d3164731/noncustodialDataSources/39383530323537383742433232433246"
}

New-MgComplianceEdiscoveryCaseSourceCollectionNoncustodialSourceByRef -CaseId $caseId -SourceCollectionId $sourceCollectionId -BodyParameter $params

```