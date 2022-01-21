---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: df5f56bc01598a83b89cd3a71cc766cc9d1f7350
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62116163"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    Number = "USPTO-3954432633"
    WebUrl = "https://patents.gov/3954432633"
}

Update-MgUserProfilePatent -UserId $userId -ItemPatentId $itemPatentId -BodyParameter $params

```