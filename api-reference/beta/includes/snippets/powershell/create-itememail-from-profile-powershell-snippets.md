---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 79c7e41e07f8367754ddbc42d933d51f0196a2a3
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62132846"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    Address = "Innocenty.Popov@adventureworks.com"
}

New-MgUserProfileEmail -UserId $userId -BodyParameter $params

```