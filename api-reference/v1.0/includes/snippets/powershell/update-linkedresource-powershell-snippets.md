---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7d9d057c36d70aefd99676abae66494fa0727392
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62128721"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    "@odata.type" = "#microsoft.graph.linkedResource"
    WebUrl = "http://microsoft.com"
    ApplicationName = "Microsoft"
    DisplayName = "Microsoft"
}

Update-MgUserTodoListTaskLinkedResource -UserId $userId -TodoTaskListId $todoTaskListId -TodoTaskId $todoTaskId -LinkedResourceId $linkedResourceId -BodyParameter $params

```