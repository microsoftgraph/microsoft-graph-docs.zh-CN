---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ae9724809581a658efbfc8d0d379ad906759a53a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62114652"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    AccountEnabled = $true
    DisplayName = "Adele Vance"
    MailNickname = "AdeleV"
    UserPrincipalName = "AdeleV@contoso.onmicrosoft.com"
    PasswordProfile = @{
        ForceChangePasswordNextSignIn = $true
        Password = "xWwvJ]6NMw+bWH-d"
    }
}

New-MgUser -BodyParameter $params

```