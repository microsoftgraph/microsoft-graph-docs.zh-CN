---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8de88cc31effe61679a06ecfc73d5f24b2bc8c25
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62106583"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    Name = "name-value"
    IsDefault = $false
}

New-MgOnPremisePublishingProfileConnectorGroup -OnPremisesPublishingProfileId $onPremisesPublishingProfileId -BodyParameter $params

```