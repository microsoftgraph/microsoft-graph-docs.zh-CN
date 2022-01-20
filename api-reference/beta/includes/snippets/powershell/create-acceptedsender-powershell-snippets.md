---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a3555194dbe92755d4b60dfb8258d7c517004bac
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62131177"
---
```powershell

Import-Module Microsoft.Graph.Groups

$params = @{
    "@odata.id" = "https://graph.microsoft.com/beta/users/alexd@contoso.com"
}

New-MgGroupAcceptedSenderByRef -GroupId $groupId -BodyParameter $params

```