---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e22312a5e25646f9c45dcf236d5c9cd2c84a3a0d
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62107935"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    DisplayName = "Travel items"
}

New-MgUserTodoList -UserId $userId -BodyParameter $params

```