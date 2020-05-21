---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 94af09c8d02ea4cfb7f769aab252d1aa89b1473e
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44334114"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var servicePrincipal = await graphClient.ServicePrincipals["delta"]
    .Request()
    .GetAsync();

```