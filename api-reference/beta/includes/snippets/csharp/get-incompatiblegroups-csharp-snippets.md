---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6a9a18a3bccff6fb3eaf69ea4757dae3514eddd378138338ee28a0f5aec3d557
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104223"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var incompatibleGroups = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackages["{accessPackage-id}"].IncompatibleGroups
    .Request()
    .GetAsync();

```