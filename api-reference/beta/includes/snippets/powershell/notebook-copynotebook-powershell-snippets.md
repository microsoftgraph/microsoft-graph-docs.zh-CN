---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 58f727217f004536fe2c7fa513c912ef67217585
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62339760"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    GroupId = "groupId-value"
    RenameAs = "renameAs-value"
}

# A UPN can also be used as -UserId.
Copy-MgUserOnenoteNotebook -UserId $userId -NotebookId $notebookId -BodyParameter $params

```