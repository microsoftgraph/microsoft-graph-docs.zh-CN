---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 08d3d8f3fab7ebe80eeeee4d37e6f43189bbee6d
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336191"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    InboundTrust = @{
        IsMfaAccepted = $true
        IsCompliantDeviceAccepted = $true
        IsHybridAzureADJoinedDeviceAccepted = $true
    }
}

Update-MgPolicyCrossTenantAccessPolicyPartner -CrossTenantAccessPolicyConfigurationPartnerTenantId $crossTenantAccessPolicyConfigurationPartnerTenantId -BodyParameter $params

```