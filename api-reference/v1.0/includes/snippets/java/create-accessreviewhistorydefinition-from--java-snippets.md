---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2803a60eae0b2c3dee2ece2286e7d73674f49447
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337653"
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
AccessReviewHistoryScheduleSettings scheduleSettings = new AccessReviewHistoryScheduleSettings();
scheduleSettings.reportRange = "P1M";
PatternedRecurrence recurrence = new PatternedRecurrence();
RecurrencePattern pattern = new RecurrencePattern();
pattern.type = RecurrencePatternType.DAILY;
pattern.interval = 1;
recurrence.pattern = pattern;
RecurrenceRange range = new RecurrenceRange();
range.type = RecurrenceRangeType.NO_END;
range.startDate = new DateOnly(1900,1,1);
range.count = 0;
recurrence.range = range;
scheduleSettings.recurrence = recurrence;
accessReviewHistoryDefinition.scheduleSettings = scheduleSettings;
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