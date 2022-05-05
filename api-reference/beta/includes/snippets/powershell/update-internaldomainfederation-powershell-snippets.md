---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bbd5f9b259bd4195869ac51af9665f50a0c85901
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211726"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    DisplayName = "Contoso name change"
    FederatedIdpMfaBehavior = "acceptIfMfaDoneByFederatedIdp"
}

Update-MgDomainFederationConfiguration -DomainId $domainId -InternalDomainFederationId $internalDomainFederationId -BodyParameter $params

```