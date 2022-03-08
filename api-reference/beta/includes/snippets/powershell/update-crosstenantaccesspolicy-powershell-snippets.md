---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 999672bab7d8772cb97bd999e80b45c8a0658f3e
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336646"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    DisplayName = "CrossTenantAccessPolicy"
}

Update-MgPolicyCrossTenantAccessPolicy -BodyParameter $params

```