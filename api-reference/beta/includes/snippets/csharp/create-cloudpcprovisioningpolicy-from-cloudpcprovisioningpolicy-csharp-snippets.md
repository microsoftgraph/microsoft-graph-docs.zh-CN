---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 307837e1d404f2ead0f978f36421a0c7ae5db1c0f829cf8b71cf8a550639610b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105480"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcProvisioningPolicy = new CloudPcProvisioningPolicy
{
    DisplayName = "Display Name value",
    Description = "Description value",
    OnPremisesConnectionId = "6bf90392-5fea-459a-9e9d-a2484abbffff",
    ImageId = "Image ID value",
    ImageDisplayName = "Image Display Name value",
    ImageType = CloudPcProvisioningPolicyImageType.Gallery
};

await graphClient.DeviceManagement.VirtualEndpoint.ProvisioningPolicies
    .Request()
    .AddAsync(cloudPcProvisioningPolicy);

```