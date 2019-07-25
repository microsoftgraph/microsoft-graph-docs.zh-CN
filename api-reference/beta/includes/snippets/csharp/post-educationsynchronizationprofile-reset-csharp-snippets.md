---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4a02b66cb311bbc274e643b5cee2c1e43b3ba883
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35712464"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.SynchronizationProfiles["{id}"]
    .Reset()
    .Request()
    .PostAsync();

```