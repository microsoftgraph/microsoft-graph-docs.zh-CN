---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9e3d384f5506736a26c561ec2a37482966e6e73de425259fac0b41c33cd9153c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333016"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Policies.PermissionGrantPolicies["{permissionGrantPolicy-id}"].Excludes["{permissionGrantConditionSet-id}"]
    .Request()
    .DeleteAsync();

```