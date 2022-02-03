---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3ef46868e989f83094938f898254d8e3f02040f1
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350275"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    Address = "Innocenty.Popov@adventureworks.com"
}

# A UPN can also be used as -UserId.
New-MgUserProfileEmail -UserId $userId -BodyParameter $params

```