---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3a6337d2b6566397853cbf95052193d0bc2180bb
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937536"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.TrustFramework.KeySets["{id}"]
    .GetActiveKey()
    .Request()
    .PostAsync();

```