---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9297c5c1f9176c389bad968323f0cf943e837b04
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63758647"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcProvisioningPolicy = new CloudPcProvisioningPolicy
{
    DisplayName = "HR provisioning policy",
    Description = "Provisioning policy for India HR employees",
    OnPremisesConnectionId = "4e47d0f6-6f77-44f0-8893-c0fe1701ffff",
    ImageId = "Image ID value",
    ImageDisplayName = "Image Display Name value",
    ImageType = CloudPcProvisioningPolicyImageType.Custom,
    WindowsSettings = new CloudPcWindowsSettings
    {
        Language = "en-US"
    }
};

await graphClient.DeviceManagement.VirtualEndpoint.ProvisioningPolicies["{cloudPcProvisioningPolicy-id}"]
    .Request()
    .UpdateAsync(cloudPcProvisioningPolicy);

```