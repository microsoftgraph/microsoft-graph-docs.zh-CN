---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ad9db42769c3a5e08f24ce53e5267965b21cb469
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439196"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackagesIncompatibleWith = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackages["{accessPackage-id}"].AccessPackagesIncompatibleWith
    .Request()
    .GetAsync();

```