---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b41607451390d7d3470f2078b916802cbf3b8fac
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62126172"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    DisplayName = "New display name"
}

Update-MgApplication -ApplicationId $applicationId -BodyParameter $params

```