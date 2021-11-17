---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3e513c4018e9fa10af76b14452e2f779db764c6fe7ee4eb02f92334e5fcaf71e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104171"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageCatalogs = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageCatalogs
    .Request()
    .GetAsync();

```