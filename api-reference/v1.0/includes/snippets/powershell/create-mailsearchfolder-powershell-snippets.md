---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b1a764447766cfd86ca79971316d5a8eabd6bf1
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62126291"
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

New-MgUserMailFolderChildFolder -UserId $userId -MailFolderId $mailFolderId -BodyParameter $params

```