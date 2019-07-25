---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 691b4ae1633ce91fa60e274e9743edd52ef72755
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724512"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var value = new List<String>()
{
    "id-value1",
    "id-value2"
};

await graphClient.Security.TiIndicators
    .DeleteTiIndicators(value)
    .Request()
    .PostAsync();

```