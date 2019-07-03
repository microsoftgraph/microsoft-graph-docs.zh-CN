---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3b1035bb4fdff81b1eab92f59750532e2bee1f41
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35463662"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var threads = await graphClient.Groups["{id}"].Conversations["{id}"].Threads
    .Request()
    .GetAsync();

```