---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 86db269f9f34e4cb89d9b9a979d36713aa05e81c
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350132"
---
```powershell

Import-Module Microsoft.Graph.Mail

$params = @{
    "@odata.type" = "microsoft.graph.mailSearchFolder"
    FilterQuery = "contains(subject, 'Analytics')"
}

# A UPN can also be used as -UserId.
Update-MgUserMailFolder -UserId $userId -MailFolderId $mailFolderId -BodyParameter $params

```