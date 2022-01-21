---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ac1493d5eee7bbf08cdcc77f4aa3fc8785dfcdd9
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62132731"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    ControlId = "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213"
    ControlTypeId = "6e4f3d20-c5c3-407f-9695-8460952bcc68"
    ProgramId = "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213"
}

New-MgProgramControl -BodyParameter $params

```