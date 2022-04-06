---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b0a4bdc1d88a2759555d81c0628a12bdaab8002b
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63759287"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Administration

$params = @{
    "@odata.type" = "#microsoft.graph.cloudPcProvisioningPolicy"
    Description = "Description value"
    DisplayName = "Display Name value"
    DomainJoinConfiguration = @{
        DomainJoinType = "hybridAzureADJoin"
        OnPremisesConnectionId = "16ee6c71-fc10-438b-88ac-daa1ccafffff"
    }
    Id = "1d164206-bf41-4fd2-8424-a3192d39ffff"
    ImageDisplayName = "Windows-10 19h1-evd"
    ImageId = "MicrosoftWindowsDesktop_Windows-10_19h1-evd"
    ImageType = "gallery"
    OnPremisesConnectionId = "4e47d0f6-6f77-44f0-8893-c0fe1701ffff"
    WindowsSettings = @{
        Language = "en-US"
    }
}

New-MgDeviceManagementVirtualEndpointProvisioningPolicy -BodyParameter $params

```