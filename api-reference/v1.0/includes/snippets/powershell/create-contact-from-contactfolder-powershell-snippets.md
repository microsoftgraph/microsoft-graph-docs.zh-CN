---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6b55b3cb5b88bf25d89b2ff246dd76a64ae962b1
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62101374"
---
```powershell

Import-Module Microsoft.Graph.PersonalContacts

$params = @{
    ParentFolderId = "parentFolderId-value"
    Birthday = [System.DateTime]::Parse("datetime-value")
    FileAs = "fileAs-value"
    DisplayName = "displayName-value"
    GivenName = "givenName-value"
    Initials = "initials-value"
}

New-MgUserContactFolderContact -UserId $userId -ContactFolderId $contactFolderId -BodyParameter $params

```