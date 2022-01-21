---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e3f9fae7d137cd458b99f53e42b54e4d7dc13228
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62112633"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    DisplayName = "Project expenses"
    Color = "preset9"
}

New-MgUserOutlookMasterCategory -UserId $userId -BodyParameter $params

```