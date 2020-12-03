---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 787f882d89a7a6d0bac530d8a7e72508e97f3ac7
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522214"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Policies.PermissionGrantPolicies["my-custom-consent-policy"].Includes["198d8d6b-ecf6-47bc-a3dd-eaa2fe0544c5"]
    .Request()
    .DeleteAsync();

```