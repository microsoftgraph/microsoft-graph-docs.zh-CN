---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 745d977d031b10d86ce19963852714af41416932
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44336827"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appRoleAssignedTo = await graphClient.ServicePrincipals["{id}"].AppRoleAssignedTo
    .Request()
    .GetAsync();

```