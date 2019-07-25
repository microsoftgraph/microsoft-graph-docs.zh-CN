---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 12dc129e35fc86d0a802c06c7e2a9fee8ae49a15
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35712443"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.SynchronizationProfiles["{id}"]
    .Start()
    .Request()
    .PostAsync();

```