---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d215fdf2b7411d22041d260481f792a10a266e1c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62118662"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    AllowedAudiences = "organization"
}

Update-MgUserProfileNote -UserId $userId -PersonAnnotationId $personAnnotationId -BodyParameter $params

```