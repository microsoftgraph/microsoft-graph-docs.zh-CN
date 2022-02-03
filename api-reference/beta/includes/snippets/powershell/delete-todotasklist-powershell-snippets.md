---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9584e934ec819311cd0b83c1abb4710a8e5dcac8
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351065"
---
```powershell

Import-Module Microsoft.Graph.Users

# A UPN can also be used as -UserId.
Remove-MgUserTodoList -UserId $userId -TodoTaskListId $todoTaskListId

```