---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 35b62a1f23ce74e0eda941f9a492d9f950edd4d1
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62132879"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    Type = "birthday"
    Date = "1980-01-08"
}

New-MgUserProfileAnniversary -UserId $userId -BodyParameter $params

```