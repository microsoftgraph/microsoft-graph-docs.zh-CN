---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 18e6c40121bee3630a8baa76c181bafa538fe6c96d95d0eeb07006f50491d3c0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903106"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleManagementPolicyAssignments = await graphClient.Policies.RoleManagementPolicyAssignments
    .Request()
    .GetAsync();

```