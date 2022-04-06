---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7a76efe4a066778fed2661396f3479a55d23feaa
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63759199"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Administration

$params = @{
    "@odata.type" = "#microsoft.graph.cloudPcProvisioningPolicy"
    DisplayName = "HR provisioning policy"
    Description = "Provisioning policy for India HR employees"
    OnPremisesConnectionId = "4e47d0f6-6f77-44f0-8893-c0fe1701ffff"
    ImageId = "Image ID value"
    ImageDisplayName = "Image Display Name value"
    ImageType = "custom"
    WindowsSettings = @{
        Language = "en-US"
    }
}

Update-MgDeviceManagementVirtualEndpointProvisioningPolicy -CloudPcProvisioningPolicyId $cloudPcProvisioningPolicyId -BodyParameter $params

```