---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5dc486b2a135437c0486918cefd0b8800a4a55b6
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62345804"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    EmailAddresses = @(
        "danas@contoso.onmicrosoft.com"
        "fannyd@contoso.onmicrosoft.com"
    )
    MailTipsOptions = "automaticReplies, mailboxFullStatus"
}

# A UPN can also be used as -UserId.
Get-MgUserMailTip -UserId $userId -BodyParameter $params

```