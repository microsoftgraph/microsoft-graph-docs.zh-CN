---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2f5ea02abe4882be9a4b69b5cb9db0a0543a89133ca4097dc8d2164a30dc4655
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219266"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcProvisioningPolicy = await graphClient.DeviceManagement.VirtualEndpoint.ProvisioningPolicies["{cloudPcProvisioningPolicy-id}"]
    .Request()
    .GetAsync();

```