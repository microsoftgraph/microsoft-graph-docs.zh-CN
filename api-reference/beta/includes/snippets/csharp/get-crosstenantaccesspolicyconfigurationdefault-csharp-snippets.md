---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f0d775f90ea9088871351c70e9340fb486964d5
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336471"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var crossTenantAccessPolicyConfigurationDefault = await graphClient.Policies.CrossTenantAccessPolicy.Default
    .Request()
    .GetAsync();

```