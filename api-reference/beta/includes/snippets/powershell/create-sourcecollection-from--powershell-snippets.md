---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 36fb8a624d5d1d581b9e4e72da49b1b75ebeca0b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62090433"
---
```powershell

Import-Module Microsoft.Graph.Compliance

$params = @{
    DisplayName = "Quarterly Financials search"
    ContentQuery = "subject:'Quarterly Financials'"
    "CustodianSources@odata.bind" = @(
        "https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/custodians/2192ca408ea2410eba3bec8ae873be6b/userSources/46384443-4137-3032-3437-363939433735"
    )
}

New-MgComplianceEdiscoveryCaseSourceCollection -CaseId $caseId -BodyParameter $params

```