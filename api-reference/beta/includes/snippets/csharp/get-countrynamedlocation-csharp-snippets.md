---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3cf3183f5ea48a6dcd3cf5f6409a2f9bda2e8636
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937129"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var namedLocation = await graphClient.ConditionalAccess.NamedLocations["1c4427fd-0885-4a3d-8b23-09a899ffa959"]
    .Request()
    .GetAsync();

```