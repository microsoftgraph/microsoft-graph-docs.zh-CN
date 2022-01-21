---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2f3c8238245dcdcb2d304b8dd642f73546ce24b7
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62116207"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    AllowedAudiences = "me"
    DisplayName = "Secret Hideout"
}

Update-MgUserProfileAddress -UserId $userId -ItemAddressId $itemAddressId -BodyParameter $params

```