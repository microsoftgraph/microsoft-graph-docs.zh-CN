---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 985386020d94f4fb74f000dd92d19de1c7e4fb27
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351496"
---
```powershell

Import-Module Microsoft.Graph.Users

# A UPN can also be used as -UserId.
Get-MgUserTodoList -UserId $userId -TodoTaskListId $todoTaskListId

```