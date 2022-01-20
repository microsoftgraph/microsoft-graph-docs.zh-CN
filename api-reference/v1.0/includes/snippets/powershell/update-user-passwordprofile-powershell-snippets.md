---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e5560cf00ff42b60f3d1d8ee5a7730060a36a41b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62110292"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    PasswordProfile = @{
        ForceChangePasswordNextSignIn = $false
        Password = "xWwvJ]6NMw+bWH-d"
    }
}

Update-MgUser -UserId $userId -BodyParameter $params

```