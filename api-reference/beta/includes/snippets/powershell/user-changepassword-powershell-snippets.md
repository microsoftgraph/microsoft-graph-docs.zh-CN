---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 29a1271a3414c5b072d68dbbcdbf722a5fa4dc2c
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62345819"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    CurrentPassword = "xWwvJ]6NMw+bWH-d"
    NewPassword = "0eM85N54wFxWwvJ]"
}

# A UPN can also be used as -UserId.
Update-MgUserPassword -UserId $userId -BodyParameter $params

```