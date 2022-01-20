---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a532899f2b7d1d917d5eb114b23304dd91a75008
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62100229"
---
```powershell

Import-Module Microsoft.Graph.Compliance

$params = @{
    DisplayName = "My Case 1"
}

New-MgComplianceEdiscoveryCase -BodyParameter $params

```