---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0f6a79831de362db402e35b4bbc27ea9c041d3f4
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62132895"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    AllowedAudiences = "organization"
    CountryCode = "NO"
}

New-MgUserProfileAccount -UserId $userId -BodyParameter $params

```