---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 655d29b698f4e00fbef44acfce2f4fbfd7616832
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62346488"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    UserIds = @(
        "04487ee0-f4f6-4e7f-8999-facc5a30e232"
        "13387ee0-f4f6-4e7f-8999-facc5120e345"
    )
}

Invoke-MgDismissRiskyUser -BodyParameter $params

```