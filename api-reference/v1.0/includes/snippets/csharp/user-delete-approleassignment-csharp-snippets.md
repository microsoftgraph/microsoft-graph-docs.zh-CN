---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3990fb30a9f78dd863300fcba38881b23a8f625a
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335041"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{id}"].AppRoleAssignments["{id}"]
    .Request()
    .DeleteAsync();

```