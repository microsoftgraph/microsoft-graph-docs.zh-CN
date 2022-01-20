---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1ee4b4ac80c8f8dcd04f567838dbe90dd84e6ae1
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62113383"
---
```powershell

Import-Module Microsoft.Graph.Groups

$params = @{
    "@odata.id" = "https://graph.microsoft.com/beta/directoryObjects/{id}"
}

New-MgGroupMemberByRef -GroupId $groupId -BodyParameter $params

```