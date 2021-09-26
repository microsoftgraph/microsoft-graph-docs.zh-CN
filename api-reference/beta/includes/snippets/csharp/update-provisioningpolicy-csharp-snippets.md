---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cc0dc1df792846211b75efaaa0bb5ccdbd241e7f903b8b5fe8fb2517cc09b8e3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220832"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcProvisioningPolicy = new CloudPcProvisioningPolicy
{
    DisplayName = "Display Name value",
    Description = "Description value",
    OnPremisesConnectionId = "4e47d0f6-6f77-44f0-8893-c0fe1701ffff",
    ImageId = "Image ID value",
    ImageDisplayName = "Image Display Name value",
    ImageType = CloudPcProvisioningPolicyImageType.Custom
};

await graphClient.DeviceManagement.VirtualEndpoint.ProvisioningPolicies["{cloudPcProvisioningPolicy-id}"]
    .Request()
    .UpdateAsync(cloudPcProvisioningPolicy);

```