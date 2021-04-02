---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6cbe01a34d4abb9d78eddf7367be0c5c689cfdca
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507214"
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