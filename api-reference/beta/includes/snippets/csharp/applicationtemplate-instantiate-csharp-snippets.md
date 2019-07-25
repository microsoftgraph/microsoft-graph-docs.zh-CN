---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 12a6fb4c469542d31e1e33ec008bde667defdd6c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35710161"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var displayName = "My custom name";

await graphClient.ApplicationTemplates["{id}"]
    .Instantiate(displayName)
    .Request()
    .PostAsync();

```