---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1a551f70ded198993039571ca1d7055c9bf311fe
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795009"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var excludes = await graphClient.Policies.PermissionGrantPolicies["{permissionGrantPolicy-id}"].Excludes
    .Request()
    .GetAsync();

```