---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f308d53f7b4ef885a51d773154cfa6dd6b3bf5ec
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62118290"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    DisplayName = "testprogram3"
    Description = "test description"
}

New-MgProgram -BodyParameter $params

```