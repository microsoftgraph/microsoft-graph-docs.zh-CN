---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ca3871cdec5b270678f25c2c8d63f0bc5bb506bc
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62096414"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    DisabledForGroup = "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
}

Update-MgOrganizationSettingItemInsight -OrganizationId $organizationId -BodyParameter $params

```