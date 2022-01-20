---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fa3be68f643f86021f5e4f44ff68fc8033b07cc7
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62095350"
---
```powershell

Import-Module Microsoft.Graph.Groups

$params = @{
    Description = "Self help community for library"
    DisplayName = "Library Assist"
    GroupTypes = @(
        "Unified"
    )
    MailEnabled = $true
    MailNickname = "library"
    SecurityEnabled = $false
}

New-MgGroup -BodyParameter $params

```