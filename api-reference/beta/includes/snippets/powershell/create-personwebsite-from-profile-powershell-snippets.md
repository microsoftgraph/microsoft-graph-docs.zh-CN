---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d2c45d2425b72f70c35996757445d1f2cf90cf7b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62123065"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    Categories = @(
        "football"
    )
    DisplayName = "Lyn Damer"
    WebUrl = "www.lyndamer.no"
}

New-MgUserProfileWebsite -UserId $userId -BodyParameter $params

```