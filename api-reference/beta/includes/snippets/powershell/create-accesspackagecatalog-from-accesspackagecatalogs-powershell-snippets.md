---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 09e3eeecbb16b11626deaa8981eb5b6b2bfdecde
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62108971"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    DisplayName = "sales"
    Description = "for employees working with sales and outside sales partners"
    IsExternallyVisible = $true
}

New-MgEntitlementManagementAccessPackageCatalog -BodyParameter $params

```