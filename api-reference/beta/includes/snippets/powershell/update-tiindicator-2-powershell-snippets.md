---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9229374808fa4cbb9c1bf60ac12478a3cfa934b2
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62115551"
---
```powershell

Import-Module Microsoft.Graph.Security

$params = @{
    AdditionalInformation = "additionalInformation-after-update"
    Confidence = 42
    Description = "description-after-update"
}

Update-MgSecurityTiIndicator -TiIndicatorId $tiIndicatorId -BodyParameter $params

```