---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5c72a577f5cca9b31fa170abaa5624f9b06b05c3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35478718"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedRole = await graphClient.PrivilegedRoles["{id}"]
    .Request()
    .GetAsync();

```