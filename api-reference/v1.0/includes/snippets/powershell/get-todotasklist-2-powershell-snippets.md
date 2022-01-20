---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2cc2ad1a7733f4c3af018aec57458aa53f2d4fe2
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62121679"
---
```powershell

Import-Module Microsoft.Graph.Users

Get-MgUserTodoList -UserId $userId -TodoTaskListId $todoTaskListId

```