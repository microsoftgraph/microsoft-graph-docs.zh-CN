---
description: 自动生成的文件。请勿修改
ms.openlocfilehash: 1832855ec21200e061e15f0e3d2e5c8b9c7aa36d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49214362"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewInstanceDecisionItem accessReviewInstanceDecisionItem = new AccessReviewInstanceDecisionItem();
accessReviewInstanceDecisionItem.decision = "Approve";
accessReviewInstanceDecisionItem.justification = "I trust this person";

graphClient.me().pendingAccessReviewInstances("70a68410-67f3-4d4c-b946-6989e050be19").decisions("654b34e7-b48f-4772-a2d4-08f1d0dd014c")
    .buildRequest()
    .patch(accessReviewInstanceDecisionItem);

```