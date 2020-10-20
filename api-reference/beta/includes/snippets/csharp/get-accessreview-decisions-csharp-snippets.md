---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a94b31f4799730cd2c12480606f4af4daa9130ea
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48612819"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var myDecisions = await graphClient.AccessReviews["2b83cc42-09db-46f6-8c6e-16fec466a82d"].MyDecisions
    .Request()
    .GetAsync();

```