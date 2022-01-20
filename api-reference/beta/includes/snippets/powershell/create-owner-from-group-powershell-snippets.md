---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f3e08c5a3beb20a91eff6c9537bad6674ca1199f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62127663"
---
```powershell

Import-Module Microsoft.Graph.Groups

$params = @{
    "@odata.id" = "https://graph.microsoft.com/beta/users/{id}"
}

New-MgGroupOwnerByRef -GroupId $groupId -BodyParameter $params

```