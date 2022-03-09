---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 25fdcba0a8051f7b07d0fb8bbb872bbb67f77e61
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63395788"
---
```powershell

Import-Module Microsoft.Graph.Groups

$params = @{
    TemplateId = "08d542b9-071f-4e16-94b0-74abb372e3d9"
    Values = @(
        @{
            Name = "AllowToAddGuests"
            Value = "false"
        }
    )
}

New-MgGroupSetting -GroupId $groupId -BodyParameter $params

```