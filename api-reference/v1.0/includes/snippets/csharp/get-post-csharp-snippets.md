---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4bdf2953d6cae9d4a7221a6be1d6fa21e4117dfa
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35739639"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var post = await graphClient.Groups["{id}"].Threads["{id}"].Posts["{id}"]
    .Request()
    .GetAsync();

```