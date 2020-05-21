---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 69c61e2aa4b2e80eee244f692e51885a4f2439f6
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44333915"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var transitiveMemberOf = await graphClient.ServicePrincipals["{id}"].TransitiveMemberOf
    .Request()
    .GetAsync();

```