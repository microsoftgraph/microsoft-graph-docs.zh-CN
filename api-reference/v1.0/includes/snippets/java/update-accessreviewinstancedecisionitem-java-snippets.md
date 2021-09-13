---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6acc941cde8d0b1672f7bd33a908e3a84f314bcd9fd9b27019222dcf479b7d37
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221194"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewInstanceDecisionItem accessReviewInstanceDecisionItem = new AccessReviewInstanceDecisionItem();
accessReviewInstanceDecisionItem.decision = "Approve";
accessReviewInstanceDecisionItem.justification = "Kathleen still needs access to the Marketing group as she works in the Marketing organization.";

graphClient.identityGovernance().accessReviews().definitions("abadf3b6-8ea4-4dea-90a5-9eac8fe93fbd").instances("4444f3b6-8ea4-4dea-90a5-9eac8fe95678").decisions("5555f3b6-8ea4-4dea-90a5-9eac8fe95555")
    .buildRequest()
    .patch(accessReviewInstanceDecisionItem);

```