---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 83d4bcb292d0a4020675fc40c82d8485a781a6a3
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35731443"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var versions = await graphClient.Sites["{site-id}"].Lists["{list-id}"].Items["{item-id}"].Versions
    .Request()
    .GetAsync();

```