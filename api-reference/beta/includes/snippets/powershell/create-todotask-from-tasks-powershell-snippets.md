---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a356dd7bc1efdc45ff419a4888ff830f5c483374
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352199"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    Title = "A new task"
    LinkedResources = @(
        @{
            WebUrl = "http://microsoft.com"
            ApplicationName = "Microsoft"
            DisplayName = "Microsoft"
        }
    )
}

# A UPN can also be used as -UserId.
New-MgUserTodoListTask -UserId $userId -TodoTaskListId $todoTaskListId -BodyParameter $params

```