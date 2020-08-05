---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f8c517f7737db4a17df9b78673f011ade8263881
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46569905"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var riskyUserHistoryItem = await graphClient.IdentityProtection.RiskyUsers["41a31b00-3b3b-42d9-8f1c-6d4f14e74c69"].History["41a31b00-3b3b-42d9-8f1c-6d4f14e74c69"]
    .Request()
    .GetAsync();

```