---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8ff4e2a38ceaa0500de976611682b36cded68cdb
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62114769"
---
```powershell

Import-Module Microsoft.Graph.Groups

$params = @{
    Description = "Library Assist"
    DisplayName = "Library Assist"
    GroupTypes = @(
        "Unified"
    )
    MailEnabled = $true
    MailNickname = "library-help"
}

Update-MgGroup -GroupId $groupId -BodyParameter $params

```