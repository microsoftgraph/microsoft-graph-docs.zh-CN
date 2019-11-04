---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 69452a2a98f10b959b830a5b51f6b5acc37a3382
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938332"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var keySets = await graphClient.TrustFramework.KeySets
    .Request()
    .GetAsync();

```