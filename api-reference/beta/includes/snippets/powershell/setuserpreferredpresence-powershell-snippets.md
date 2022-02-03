---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b9895bd9d7d4e8c9e5298234b163085aa39f4fd
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62344937"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    Availability = "DoNotDisturb"
    Activity = "DoNotDisturb"
    ExpirationDuration = "PT8H"
}

Set-MgUserPresenceUserPreferredPresence -UserId $userId -BodyParameter $params

```