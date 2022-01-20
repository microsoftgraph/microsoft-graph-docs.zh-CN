---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cd83ca09fd8bfcc77808f05fc936c140697f40d6
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62092751"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    CountryCode = "NO"
}

Update-MgUserProfileAccount -UserId $userId -UserAccountInformationId $userAccountInformationId -BodyParameter $params

```