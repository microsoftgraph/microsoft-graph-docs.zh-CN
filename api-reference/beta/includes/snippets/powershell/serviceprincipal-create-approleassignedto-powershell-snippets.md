---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dd25ce1f60adb25b765a0326b8c5eb33d45ea658
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62105358"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    PrincipalId = "33ad69f9-da99-4bed-acd0-3f24235cb296"
    ResourceId = "9028d19c-26a9-4809-8e3f-20ff73e2d75e"
    AppRoleId = "ef7437e6-4f94-4a0a-a110-a439eb2aa8f7"
}

New-MgServicePrincipalAppRoleAssignedTo -ServicePrincipalId $servicePrincipalId -BodyParameter $params

```