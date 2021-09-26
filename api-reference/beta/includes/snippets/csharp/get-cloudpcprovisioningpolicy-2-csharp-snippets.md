---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d34fafa8109f1d134768b7525d034a9f1be7f3ac4613a4b72b169a137ab1eec9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163828"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcProvisioningPolicy = await graphClient.DeviceManagement.VirtualEndpoint.ProvisioningPolicies["{cloudPcProvisioningPolicy-id}"]
    .Request()
    .Expand("assignments")
    .GetAsync();

```