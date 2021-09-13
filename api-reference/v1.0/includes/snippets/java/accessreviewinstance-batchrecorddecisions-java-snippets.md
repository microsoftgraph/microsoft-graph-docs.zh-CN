---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9fd9a4988d5057ba5c190e52c6a2eb93b9b33e28f4ea2ae7104b0bb66c2400b2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277194"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String decision = "Approve";

String justification = "All principals with access need continued access to the resource (Marketing Group) as all the principals are on the marketing team";

String resourceId = "a5c51e59-3fcd-4a37-87a1-835c0c21488a";

graphClient.identityGovernance().accessReviews().definitions("e6cafba0-cbf0-4748-8868-0810c7f4cc06").instances("1234fba0-cbf0-6778-8868-9999c7f4cc06")
    .batchRecordDecisions(AccessReviewInstanceBatchRecordDecisionsParameterSet
        .newBuilder()
        .withDecision(decision)
        .withJustification(justification)
        .withPrincipalId(null)
        .withResourceId(resourceId)
        .build())
    .buildRequest()
    .post();

```