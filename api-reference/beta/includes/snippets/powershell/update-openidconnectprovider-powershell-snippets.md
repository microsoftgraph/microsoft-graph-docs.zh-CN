---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d9bca7eff54feb24c674fadfb93225d71ddcb820
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2022
ms.locfileid: "62225762"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    ResponseType = "id_token"
}

Update-MgIdentityProvider -IdentityProviderId $identityProviderId -BodyParameter $params

```