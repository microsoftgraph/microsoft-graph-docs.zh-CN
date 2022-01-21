---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9676836d51b6ff7cc31d7658f9073af82ed78b8b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62100950"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    DisplayName = "sales reps"
    Description = "outside sales representatives"
    IsHidden = $false
    Catalog = @{
        Id = "66584aae-98bb-48cc-9458-7bee5d2a6577"
    }
}

New-MgEntitlementManagementAccessPackage -BodyParameter $params

```