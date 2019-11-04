---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 133a06f2785a26819ee8a55a28e0c9ff80b6f6fb
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938612"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityUserFlow = await graphClient.Identity.UserFlows["B2C_1_Pol1"]
    .Request()
    .GetAsync();

```