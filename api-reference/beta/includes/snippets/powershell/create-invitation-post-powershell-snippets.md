---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7988667217f10dc26c016c1151e968da4a8189fe
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62129812"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    InvitedUserEmailAddress = "admin@fabrikam.com"
    InviteRedirectUrl = "https://myapp.contoso.com"
}

New-MgInvitation -BodyParameter $params

```