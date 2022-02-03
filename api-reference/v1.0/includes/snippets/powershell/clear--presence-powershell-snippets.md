---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 03557e97c38d2ebf737f0bedd5652fa83e220396
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62348621"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    SessionId = "22553876-f5ab-4529-bffb-cfe50aa89f87"
}

Clear-MgUserPresence -UserId $userId -BodyParameter $params

```