---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1a7367d3993dad0e4476ee168c356d13bab052e4
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507474"
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