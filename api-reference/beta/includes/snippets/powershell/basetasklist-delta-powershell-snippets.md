---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d9def03784ed78db77de74bd3c6f9b7ec23b182c
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62343550"
---
```powershell

Import-Module Microsoft.Graph.Users.Functions

# A UPN can also be used as -UserId.
Get-MgUserTaskListDelta -UserId $userId

```