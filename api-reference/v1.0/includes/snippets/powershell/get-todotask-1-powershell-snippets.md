---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b2a4e9727145df0529a0c8a9aca24db49048d058
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62091540"
---
```powershell

Import-Module Microsoft.Graph.Users

Get-MgUserTodoListTask -UserId $userId -TodoTaskListId $todoTaskListId -TodoTaskId $todoTaskId

```