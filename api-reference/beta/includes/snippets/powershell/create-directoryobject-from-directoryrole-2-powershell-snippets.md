---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 034960ea7948fa967e70344fee3f073ee2dfd669
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62094221"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    "@odata.id" = "https://graph.microsoft.com/beta/directoryObjects/2c891f12-928d-4da2-8d83-7d2434a0d8dc"
}

New-MgDirectoryRoleMemberByRef -DirectoryRoleId $directoryRoleId -BodyParameter $params

```