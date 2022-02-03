---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d48a174e82544383024b599fdecb8e8bd282a5cc
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62346124"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    Key = "key-value"
}

Invoke-MgUploadTrustFrameworkKeySetCertificate -TrustFrameworkKeySetId $trustFrameworkKeySetId -BodyParameter $params

```