---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: af24a301edafcde97692e6377e30658e19546e1f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62107963"
---
```powershell

Import-Module Microsoft.Graph.Users

Get-MgUserTodoListTaskLinkedResource -UserId $userId -TodoTaskListId $todoTaskListId -TodoTaskId $todoTaskId

```