---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f3d9a31085b7c64beb4c3b77dfce722b3195be8f
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350179"
---
```powershell

Import-Module Microsoft.Graph.Mail

$params = @{
    ReceivedDateTime = [System.DateTime]::Parse("2016-10-19T10:37:00Z")
    SentDateTime = [System.DateTime]::Parse("2016-10-19T10:37:00Z")
    HasAttachments = $true
    Subject = "subject-value"
    Body = @{
        ContentType = ""
        Content = "content-value"
    }
    BodyPreview = "bodyPreview-value"
}

# A UPN can also be used as -UserId.
New-MgUserMailFolderMessage -UserId $userId -MailFolderId $mailFolderId -BodyParameter $params

```