---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7591d75eeaf26af1760a6c64d97c867813dc6611
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62095837"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    Id = "SCIM-Test1"
    ApplicationId = "{id}"
    FactoryTag = "CustomSCIM"
}

New-MgApplicationSynchronizationTemplate -ApplicationId $applicationId -BodyParameter $params

```