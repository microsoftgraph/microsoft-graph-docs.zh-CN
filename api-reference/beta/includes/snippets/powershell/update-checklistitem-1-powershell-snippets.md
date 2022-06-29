---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a53783f36547496e4928ad8d6662f298c28e9d0d
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66436247"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    DisplayName = "buy cake"
}

# A UPN can also be used as -UserId.
Update-MgUserTodoListTaskChecklistItem -UserId $userId -TodoTaskListId $todoTaskListId -TodoTaskId $todoTaskId -ChecklistItemId $checklistItemId -BodyParameter $params

```