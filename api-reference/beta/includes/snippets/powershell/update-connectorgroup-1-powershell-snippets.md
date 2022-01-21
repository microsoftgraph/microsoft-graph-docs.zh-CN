---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b6591c200b5fcb6068ff1cb1ce3231f48cab9ceb
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62097119"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    Name = "Connector Group Demo"
}

New-MgOnPremisePublishingProfileConnectorGroup -OnPremisesPublishingProfileId $onPremisesPublishingProfileId -BodyParameter $params

```