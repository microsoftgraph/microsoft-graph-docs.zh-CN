---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0f0459a24fda24b2abd1a395e3bc2b6923e8937f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62136490"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    "@odata.id" = "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}

New-MgApplicationOwnerByRef -ApplicationId $applicationId -BodyParameter $params

```