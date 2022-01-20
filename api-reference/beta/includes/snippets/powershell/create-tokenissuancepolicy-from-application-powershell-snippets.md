---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 91f62eb2eb21f736ef302a499097d808b0138265
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62090931"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    "@odata.id" = "https://graph.microsoft.com/beta/policies/tokenIssuancePolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"
}

New-MgApplicationTokenIssuancePolicyByRef -ApplicationId $applicationId -BodyParameter $params

```