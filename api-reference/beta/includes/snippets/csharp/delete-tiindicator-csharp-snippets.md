---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5ff62041649bb1ebf8589c4686f85c592961b7de
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35716924"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Security.TiIndicators["{id}"]
    .Request()
    .DeleteAsync();

```