---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b0af37a4f823a53a2a9148bd7dcd2191d2bc84be
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62101164"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    IsDefault = $true
    SupportedServices = @(
        "Email"
        "OfficeCommunicationsOnline"
    )
}

Update-MgDomain -DomainId $domainId -BodyParameter $params

```