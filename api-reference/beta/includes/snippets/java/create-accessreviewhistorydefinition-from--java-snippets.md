---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 92d6582f4465002a3198850cb985ae8010507776d4d2c0c751a2a14c8414e65a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902693"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewHistoryDefinition accessReviewHistoryDefinition = new AccessReviewHistoryDefinition();
accessReviewHistoryDefinition.displayName = "Last quarter's group reviews April 2021";
LinkedList<AccessReviewHistoryDecisionFilter> decisionsList = new LinkedList<AccessReviewHistoryDecisionFilter>();
decisionsList.add(AccessReviewHistoryDecisionFilter.APPROVE);
decisionsList.add(AccessReviewHistoryDecisionFilter.DENY);
decisionsList.add(AccessReviewHistoryDecisionFilter.DONT_KNOW);
decisionsList.add(AccessReviewHistoryDecisionFilter.NOT_REVIEWED);
decisionsList.add(AccessReviewHistoryDecisionFilter.NOT_NOTIFIED);
accessReviewHistoryDefinition.decisions = decisionsList;
accessReviewHistoryDefinition.reviewHistoryPeriodStartDateTime = OffsetDateTimeSerializer.deserialize("2021-01-01T00:00:00Z");
accessReviewHistoryDefinition.reviewHistoryPeriodEndDateTime = OffsetDateTimeSerializer.deserialize("2021-04-05T00:00:00Z");
LinkedList<AccessReviewScope> scopesList = new LinkedList<AccessReviewScope>();
AccessReviewQueryScope scopes = new AccessReviewQueryScope();
scopes.queryType = "MicrosoftGraph";
scopes.query = "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, 'accessPackageAssignments')";
scopes.queryRoot = null;
scopesList.add(scopes);
AccessReviewQueryScope scopes1 = new AccessReviewQueryScope();
scopes1.queryType = "MicrosoftGraph";
scopes1.query = "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups')";
scopes1.queryRoot = null;
scopesList.add(scopes1);
accessReviewHistoryDefinition.scopes = scopesList;

graphClient.identityGovernance().accessReviews().historyDefinitions()
    .buildRequest()
    .post(accessReviewHistoryDefinition);

```