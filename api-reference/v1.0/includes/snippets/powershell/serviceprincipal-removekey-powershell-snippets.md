---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dff2cc1642081e2b487cf3380ea35dbe25443829
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62344124"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    KeyId = "f0b0b335-1d71-4883-8f98-567911bfdca6"
    Proof = "eyJ0eXAiOiJ..."
}

Remove-MgServicePrincipalKey -ServicePrincipalId $servicePrincipalId -BodyParameter $params

```