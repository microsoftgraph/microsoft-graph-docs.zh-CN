---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 71367c86d21e774e344045d9624eb7c07d31ba6d
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524382"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Policies.PermissionGrantPolicies["my-custom-consent-policy"].Excludes["6a846635-3e70-4a10-821e-512a0db93cbd"]
    .Request()
    .DeleteAsync();

```