---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 17f262255138dc69e0bbe352dfd2a82b097f172f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799638"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Policies.PermissionGrantPolicies["{permissionGrantPolicy-id}"]
    .Request()
    .DeleteAsync();

```