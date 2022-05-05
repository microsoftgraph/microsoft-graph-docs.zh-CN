---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 00e24d9b9cd325f4dbb3bb8c627d2593589031bb
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65203834"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var incompatibleAccessPackages = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackages["{accessPackage-id}"].IncompatibleAccessPackages
    .Request()
    .GetAsync();

```