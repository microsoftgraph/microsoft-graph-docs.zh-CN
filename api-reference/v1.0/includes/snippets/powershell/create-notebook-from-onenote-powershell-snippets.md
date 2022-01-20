---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 22b3b19eb70b1e36cae6d34353af5fce14b1a0d4
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62132395"
---
```powershell

Import-Module Microsoft.Graph.Notes

$params = @{
    DisplayName = "My Private notebook"
}

New-MgUserOnenoteNotebook -UserId $userId -BodyParameter $params

```