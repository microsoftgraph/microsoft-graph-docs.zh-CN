---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bdc68771f5bf40ffed46298a8bbd2b6a26b9e1485872eb268c1e002bb59e9021
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158602"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String decision = "Approve";

String justification = "All principals with access need continued access to the resource (Marketing Group) as all the principals are on the marketing team";

String resourceId = "a5c51e59-3fcd-4a37-87a1-835c0c21488a";

graphClient.me().pendingAccessReviewInstances("{accessReviewInstanceId}")
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