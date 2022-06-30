---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c2a65ea7892d4860e7a9e04c600d41373560f8a
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66440075"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    "@odata.id" = "https://graph.microsoft.com/beta/users/{id}"
}

New-MgEntitlementManagementConnectedOrganizationExternalSponsorByRef -ConnectedOrganizationId $connectedOrganizationId -BodyParameter $params

```