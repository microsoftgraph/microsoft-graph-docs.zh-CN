---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ee530ca4a7ac095b22f69d031b938ac2c7a8348f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62118026"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    CustomSecurityAttributes = @{
        Engineering = @{
            "@odata.type" = "#Microsoft.DirectoryServices.CustomSecurityAttributeValue"
            ProjectDate = "2022-10-01"
        }
    }
}

Update-MgUser -UserId $userId -BodyParameter $params

```