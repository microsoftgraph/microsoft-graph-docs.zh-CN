---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d5c25f86ec4c13ba250bd1f82160fa591d87ab05
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62110478"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    DueDateTime = @{
        DateTime = "2020-07-25T16:00:00"
        TimeZone = "Eastern Standard Time"
    }
}

Update-MgUserTodoListTask -UserId $userId -TodoTaskListId $todoTaskListId -TodoTaskId $todoTaskId -BodyParameter $params

```