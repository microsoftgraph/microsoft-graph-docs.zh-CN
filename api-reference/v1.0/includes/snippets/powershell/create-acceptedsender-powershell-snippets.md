---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 83b740011f8c6bbb935ef42d3d566e363f23fb0b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62088479"
---
```powershell

Import-Module Microsoft.Graph.Groups

$params = @{
    "@odata.id" = "https://graph.microsoft.com/v1.0/users/alexd@contoso.com"
}

New-MgGroupAcceptedSenderByRef -GroupId $groupId -BodyParameter $params

```