---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3c0ef9e3d0222b6fef52157c91f74f0c9da2f493
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62132479"
---
```powershell

Import-Module Microsoft.Graph.Mail

$params = @{
    ReceivedDateTime = [System.DateTime]::Parse("datetime-value")
    SentDateTime = [System.DateTime]::Parse("datetime-value")
    HasAttachments = $true
    Subject = "subject-value"
    Body = @{
        ContentType = ""
        Content = "content-value"
    }
    BodyPreview = "bodyPreview-value"
}

New-MgUserMailFolderMessage -UserId $userId -MailFolderId $mailFolderId -BodyParameter $params

```