---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 84532a42076609dca9e1c7db148cf523ea0d573e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62099638"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    Id = "Pol1"
    UserFlowType = "signUpOrSignIn"
    UserFlowTypeVersion = 1
}

New-MgIdentityUserFlow -BodyParameter $params

```