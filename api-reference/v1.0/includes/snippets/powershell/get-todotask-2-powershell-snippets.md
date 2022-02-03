---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f955ebef4d4ca1a1c7875dfdaef9eaf5d7cddcb7
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350004"
---
```powershell

Import-Module Microsoft.Graph.Users

# A UPN can also be used as -UserId.
Get-MgUserTodoListTask -UserId $userId -TodoTaskListId $todoTaskListId

```