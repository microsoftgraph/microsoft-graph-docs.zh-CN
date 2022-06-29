---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cc224cd3b507302f86d8d39e094d4b7daef68a5f
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66436799"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    DisplayName = "Final sign-off from the team"
}

# A UPN can also be used as -UserId.
New-MgUserTodoListTaskChecklistItem -UserId $userId -TodoTaskListId $todoTaskListId -TodoTaskId $todoTaskId -BodyParameter $params

```