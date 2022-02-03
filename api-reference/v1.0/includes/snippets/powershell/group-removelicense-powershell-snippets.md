---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 027fa9f63998a4667818008d0bea41abeb126589
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62340839"
---
```powershell

Import-Module Microsoft.Graph.Groups

$params = @{
    AddLicenses = @(
    )
    RemoveLicenses = @(
        "c7df2760-2c81-4ef7-b578-5b5392b571df"
        "b05e124f-c7cc-45a0-a6aa-8cf78c946968"
    )
}

Set-MgGroupLicense -GroupId $groupId -BodyParameter $params

```