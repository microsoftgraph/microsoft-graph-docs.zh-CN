---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c5573a71245fb9d748d2df04a3c81076a5f061690da05e63949d7865e948dc31
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902757"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageResourceEnvironment = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageResourceEnvironments["{accessPackageResourceEnvironment-id}"]
    .Request()
    .GetAsync();

```