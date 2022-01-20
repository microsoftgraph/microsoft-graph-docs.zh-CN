---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 593cf26b26db35148ed5e88f9d13d1810139dce1
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62130709"
---
```powershell

Import-Module Microsoft.Graph.Users

Remove-MgUserTodoListTask -UserId $userId -TodoTaskListId $todoTaskListId -TodoTaskId $todoTaskId

```