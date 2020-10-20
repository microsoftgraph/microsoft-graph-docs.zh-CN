---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3debe5217c9da100fb7d53bbd05722f7ae47a227
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48608028"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityRiskEvents = await graphClient.IdentityRiskEvents
    .Request()
    .GetAsync();

```