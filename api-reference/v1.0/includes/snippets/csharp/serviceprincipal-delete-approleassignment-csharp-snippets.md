---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6f854d73d2c929752c4539c96637525b115a946b
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44334215"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.ServicePrincipals["{id}"].AppRoleAssignments["{id}"]
    .Request()
    .DeleteAsync();

```