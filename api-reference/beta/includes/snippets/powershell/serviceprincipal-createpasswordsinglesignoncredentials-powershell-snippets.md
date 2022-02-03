---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 54cb4f22a3b2a42b214bf141d7c64addefed0587
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62340988"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    Id = "5793aa3b-cca9-4794-679a240f8b58"
    Credentials = @(
        @{
            FieldId = "param_username"
            Value = "myusername"
            Type = "username"
        }
        @{
            FieldId = "param_password"
            Value = "pa$$w0rd"
            Type = "password"
        }
    )
}

New-MgServicePrincipalPasswordSingleSignOnCredentials -ServicePrincipalId $servicePrincipalId -BodyParameter $params

```