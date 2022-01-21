---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b9e22e8557bd2f68573b5472fe4deafc26747de2
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62132802"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    DisplayName = "Car Phone"
    Number = "+7 499 342 22 13"
}

New-MgUserProfilePhone -UserId $userId -BodyParameter $params

```