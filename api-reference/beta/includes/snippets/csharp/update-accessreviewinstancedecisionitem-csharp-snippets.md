---
description: 自动生成的文件。请勿修改
ms.openlocfilehash: 72e96a0f931c9e4fb9a83f1f9c15c9047d09b1fd
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49214330"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessReviewInstanceDecisionItem = new AccessReviewInstanceDecisionItem
{
    Decision = "Approve",
    Justification = "I trust this person"
};

await graphClient.Me.PendingAccessReviewInstances["70a68410-67f3-4d4c-b946-6989e050be19"].Decisions["654b34e7-b48f-4772-a2d4-08f1d0dd014c"]
    .Request()
    .UpdateAsync(accessReviewInstanceDecisionItem);

```