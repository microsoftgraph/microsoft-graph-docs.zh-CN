---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 38e594b27b6c09cb074a435adfc500ab16e6f3d8
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209616"
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