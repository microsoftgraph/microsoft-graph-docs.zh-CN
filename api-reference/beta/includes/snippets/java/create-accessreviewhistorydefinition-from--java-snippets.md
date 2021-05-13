---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f9ff71ff574afe3974045e85b1386a600de627a7
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474107"
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