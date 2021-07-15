---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 169a34c352741a35f8438e14747df0436020919c
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439403"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.IdentityGovernance.EntitlementManagement.AccessPackages["{accessPackage-id}"].IncompatibleGroups["{group-id}"].Reference
    .Request()
    .DeleteAsync();

```