---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8747b2ce8f449c7ad53685f5f8b826c09c9d221c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35712543"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.SynchronizationProfiles["{id}"]
    .Request()
    .DeleteAsync();

```