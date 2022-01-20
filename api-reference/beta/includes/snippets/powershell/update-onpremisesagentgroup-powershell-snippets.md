---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 30ac3a130fb50e1218ed6b9e299b7be7043803c7
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62135427"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    DisplayName = "Group New Name"
}

Update-MgOnPremisePublishingProfileAgentGroup -OnPremisesPublishingProfileId $onPremisesPublishingProfileId -OnPremisesAgentGroupId $onPremisesAgentGroupId -BodyParameter $params

```