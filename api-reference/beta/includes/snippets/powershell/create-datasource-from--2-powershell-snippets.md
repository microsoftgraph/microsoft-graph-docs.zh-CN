---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e366ff6228e9102ef467ecae22aa4db7535a5f41
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62120818"
---
```powershell

Import-Module Microsoft.Graph.Compliance

$params = @{
    "@odata.id" = "https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/custodians/ab3a628a383045eba344b3caecba3104/userSources/31423539-3846-4333-4136-353644383531"
}

New-MgComplianceEdiscoveryCaseSourceCollectionCustodianSourceByRef -CaseId $caseId -SourceCollectionId $sourceCollectionId -BodyParameter $params

```