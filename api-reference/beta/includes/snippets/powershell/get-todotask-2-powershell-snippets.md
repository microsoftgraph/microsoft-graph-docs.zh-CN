---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b98870a69aa7a30b45985194c6929dc288df867e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62136918"
---
```powershell

Import-Module Microsoft.Graph.Users

Get-MgUserTodoListTask -UserId $userId -TodoTaskListId $todoTaskListId

```