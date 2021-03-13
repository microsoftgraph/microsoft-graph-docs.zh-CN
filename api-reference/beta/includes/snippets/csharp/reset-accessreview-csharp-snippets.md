---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0171003dd58b2cc61bece35033c913d2e4435418
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783252"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.AccessReviews["{accessReview-id}"]
    .ResetDecisions()
    .Request()
    .PostAsync();

```