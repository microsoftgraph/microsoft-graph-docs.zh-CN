---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 26afaa3da11b5986c2ad9bc7ea2f83e4bca401d9
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352172"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    DisplayName = "Vacation Plan"
}

# A UPN can also be used as -UserId.
Update-MgUserTodoList -UserId $userId -TodoTaskListId $todoTaskListId -BodyParameter $params

```