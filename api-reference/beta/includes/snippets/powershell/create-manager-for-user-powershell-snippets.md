---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6d1301b373463cf89d180ecc5b8d0f0a61c14cff
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65719276"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    "@odata.id" = "https://graph.microsoft.com/beta/users/6ea91a8d-e32e-41a1-b7bd-d2d185eed0e0"
}

Set-MgUserManagerByRef -UserId $userId -BodyParameter $params

```