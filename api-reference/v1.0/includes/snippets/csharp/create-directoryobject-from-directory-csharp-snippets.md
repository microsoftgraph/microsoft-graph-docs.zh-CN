---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2621d5fc0bbf6b6509bcf3b340b38217354b5b19
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35737950"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Directory.DeletedItems["{object-id}"]
    .Restore()
    .Request()
    .PostAsync();

```