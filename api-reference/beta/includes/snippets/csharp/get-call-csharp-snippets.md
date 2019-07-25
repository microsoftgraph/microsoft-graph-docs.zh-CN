---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f7b26893333fb502127daf0440e51a5e0efe44ff
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35708958"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var Call = await graphClient.App.Calls["{id}"]
    .Request()
    .GetAsync();

```