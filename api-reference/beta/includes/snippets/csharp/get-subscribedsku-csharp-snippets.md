---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 27243f32ce1690c651ae094c08e99b2c75415507
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725115"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var subscribedSku = await graphClient.SubscribedSkus["{id}"]
    .Request()
    .GetAsync();

```