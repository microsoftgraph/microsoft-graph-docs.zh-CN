---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c2662ba6d599a13937ef7a835f9691f112c8edd2
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62135231"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    DisplayName = "Innocenty Popov"
    First = "Innocenty"
    Initials = "IP"
    Last = "Popov"
    LanguageTag = "en-US"
    Maiden = $null
}

New-MgUserProfileName -UserId $userId -BodyParameter $params

```