---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c17ab0ac845438cd14137f62d655018fdb0c94adeeb6d1e1847a3202df1c9cd8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902654"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewInstanceDecisionItem accessReviewInstanceDecisionItem = new AccessReviewInstanceDecisionItem();
accessReviewInstanceDecisionItem.decision = "Approve";
accessReviewInstanceDecisionItem.justification = "This person is still on my team";

graphClient.me().pendingAccessReviewInstances("70a68410-67f3-4d4c-b946-6989e050be19").decisions("12348410-67f3-4d4c-b946-6989e050be19")
    .buildRequest()
    .patch(accessReviewInstanceDecisionItem);

```