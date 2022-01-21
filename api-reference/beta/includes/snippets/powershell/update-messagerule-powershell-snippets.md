---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 94885a9a555a7754df101e5e9f31b34733589a0d
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62105799"
---
```powershell

Import-Module Microsoft.Graph.Mail

$params = @{
    DisplayName = "Important from partner"
    Actions = @{
        MarkImportance = "high"
    }
}

Update-MgUserMailFolderMessageRule -UserId $userId -MailFolderId $mailFolderId -MessageRuleId $messageRuleId -BodyParameter $params

```