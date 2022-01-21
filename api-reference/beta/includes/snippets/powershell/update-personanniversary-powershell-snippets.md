---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f4be50a6dcd4cb9fadcf24461ccb286355432dad
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137058"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    AllowedAudiences = "contacts"
}

Update-MgUserProfileAnniversary -UserId $userId -PersonAnnualEventId $personAnnualEventId -BodyParameter $params

```