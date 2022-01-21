---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e970c3556a4b2aa1e4d0a5d50e8b257178c71e06
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62096413"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    IsEnabledInOrganization = $true
    DisabledForGroup = "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
}

Update-MgOrganizationSettingPersonInsight -OrganizationId $organizationId -BodyParameter $params

```