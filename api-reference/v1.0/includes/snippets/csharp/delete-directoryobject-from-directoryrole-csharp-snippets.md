---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 84c69da79d55b661e0791e650beb7868e7a570bc
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35734032"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.DirectoryRoles["{id}"].Members["{id}"].Reference
    .Request()
    .DeleteAsync();

```