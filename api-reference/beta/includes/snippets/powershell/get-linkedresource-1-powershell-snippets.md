---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: df5c8570dcbba7211e7ca535ed10e9d87051f7f7
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62089896"
---
```powershell

Import-Module Microsoft.Graph.Users

Get-MgUserTodoListTaskLinkedResource -UserId $userId -TodoTaskListId $todoTaskListId -TodoTaskId $todoTaskId -LinkedResourceId $linkedResourceId

```