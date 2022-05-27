---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1e2e39fab3bd0c1e84c8f8fcaa9e771c86bc581b
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65719241"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    "@odata.id" = "https://graph.microsoft.com/v1.0/users/6ea91a8d-e32e-41a1-b7bd-d2d185eed0e0"
}

Set-MgUserManagerByRef -UserId $userId -BodyParameter $params

```