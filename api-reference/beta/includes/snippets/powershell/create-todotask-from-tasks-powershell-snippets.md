---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1354655cacd387c79dd5eeaa1bb10c8a39524c4e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62093038"
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

New-MgUserTodoListTask -UserId $userId -TodoTaskListId $todoTaskListId -BodyParameter $params

```