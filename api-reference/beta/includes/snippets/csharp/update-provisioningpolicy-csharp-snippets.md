---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d480473a794074d168b5cae9fa4f42c4b3953e3e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62131445"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcProvisioningPolicy = new CloudPcProvisioningPolicy
{
    DisplayName = "HR provisioning policy",
    Description = "Provisioning policy for India HR employees",
    OnPremisesConnectionId = "4e47d0f6-6f77-44f0-8893-c0fe1701b553"
};

await graphClient.DeviceManagement.VirtualEndpoint.ProvisioningPolicies["{cloudPcProvisioningPolicy-id}"]
    .Request()
    .UpdateAsync(cloudPcProvisioningPolicy);

```