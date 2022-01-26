---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0175b255d2c328067cb185f9bcce1fb816676c35
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2022
ms.locfileid: "62225141"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String decision = "Deny";

String justification = "Alice switched teams and no longer works with this group";

String principalId = "2043848d-e422-473c-8607-88a3319ff491";

String resourceId = "733ef921-89e1-4d7e-aeff-83612223c37e";

graphClient.identityGovernance().accessReviews().decisions()
    .filterByCurrentUser(AccessReviewInstanceDecisionItemFilterByCurrentUserParameterSet
        .newBuilder()
        .withOn(null)
        .build())
    .recordAllDecisions(AccessReviewInstanceDecisionItemRecordAllDecisionsParameterSet
        .newBuilder()
        .withDecision(decision)
        .withJustification(justification)
        .withPrincipalId(principalId)
        .withResourceId(resourceId)
        .build())
    .buildRequest()
    .post();

```