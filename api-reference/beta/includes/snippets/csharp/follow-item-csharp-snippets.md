---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4f82cb90fcecd47d6f218a9d12b1dfa6a1908264
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35712913"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{item-id}"]
    .Follow()
    .Request()
    .PostAsync();

```