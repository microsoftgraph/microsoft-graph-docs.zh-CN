---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d9c028aff50f9be28e05e42b70382b0264a9cedc
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62339809"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    DestinationId = "destinationId-value"
}

# A UPN can also be used as -UserId.
Copy-MgUserMailFolder -UserId $userId -MailFolderId $mailFolderId -BodyParameter $params

```