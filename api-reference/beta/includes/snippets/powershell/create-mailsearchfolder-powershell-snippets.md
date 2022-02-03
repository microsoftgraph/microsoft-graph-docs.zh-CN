---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c1b92e175fc71299bc11207f30392850181f4721
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349594"
---
```powershell

Import-Module Microsoft.Graph.Mail

$params = @{
    "@odata.type" = "microsoft.graph.mailSearchFolder"
    DisplayName = "Weekly digests"
    IncludeNestedFolders = $true
    SourceFolderIds = @(
        "AQMkADYAAAIBDAAAAA=="
    )
    FilterQuery = "contains(subject, 'weekly digest')"
}

# A UPN can also be used as -UserId.
New-MgUserMailFolderChildFolder -UserId $userId -MailFolderId $mailFolderId -BodyParameter $params

```