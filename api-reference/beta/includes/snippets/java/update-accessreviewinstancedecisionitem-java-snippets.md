---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b280f4368d9f86a2b8f8074d50d44578b2765d3
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/16/2022
ms.locfileid: "62855753"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewInstanceDecisionItem accessReviewInstanceDecisionItem = new AccessReviewInstanceDecisionItem();
accessReviewInstanceDecisionItem.decision = "Approve";
accessReviewInstanceDecisionItem.justification = "This person is still on my team";

graphClient.identityGovernance().accessReviews().definitions("5eac5a70-7cd7-4f20-92b0-f9dba70dd7f0").instances("6444d4fd-ab55-4608-8cf9-c6702d172bcc").stages("9458f255-dff2-4d86-9a05-69438f49d7f8").decisions("e6cafba0-cbf0-4748-8868-0810c7f4cc06")
    .buildRequest()
    .patch(accessReviewInstanceDecisionItem);

```