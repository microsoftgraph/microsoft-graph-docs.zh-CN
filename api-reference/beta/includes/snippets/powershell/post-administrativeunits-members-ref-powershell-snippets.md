---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 06a635f3265e4cb52fd7ff4b5b4411bd309ac507
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62097398"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    "@odata.id" = "https://graph.microsoft.com/beta/groups/{id}"
}

New-MgAdministrativeUnitMemberByRef -AdministrativeUnitId $administrativeUnitId -BodyParameter $params

```