---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4db70ef8a7e22bdbce51854a427ff1cac05ac0c8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972752"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewScheduleDefinition accessReviewScheduleDefinition = new AccessReviewScheduleDefinition();
accessReviewScheduleDefinition.displayName = "Test create";
accessReviewScheduleDefinition.descriptionForAdmins = "New scheduled access review";
accessReviewScheduleDefinition.descriptionForReviewers = "If you have any questions, contact jerry@contoso.com";
AccessReviewScope scope = new AccessReviewScope();
scope.query = "/groups/b7a059cb-038a-4802-8fc9-b9d1ed0c4444/transitiveMembers";
scope.queryType = "MicrosoftGraph";
accessReviewScheduleDefinition.scope = scope;
LinkedList<AccessReviewReviewerScope> reviewersList = new LinkedList<AccessReviewReviewerScope>();
AccessReviewReviewerScope reviewers = new AccessReviewReviewerScope();
reviewers.query = "/users/7eae4444-d425-48b2-adf2-3c777f6256f3";
reviewers.queryType = "MicrosoftGraph";
reviewers.queryRoot = "decisions";
reviewersList.add(reviewers);
accessReviewScheduleDefinition.reviewers = reviewersList;
AccessReviewScheduleSettings settings = new AccessReviewScheduleSettings();
settings.mailNotificationsEnabled = true;
settings.reminderNotificationsEnabled = true;
settings.justificationRequiredOnApproval = true;
settings.defaultDecisionEnabled = false;
settings.defaultDecision = "None";
settings.instanceDurationInDays = 1;
settings.autoApplyDecisionsEnabled = false;
settings.recommendationsEnabled = true;
PatternedRecurrence recurrence = new PatternedRecurrence();
RecurrencePattern pattern = new RecurrencePattern();
pattern.type = RecurrencePatternType.WEEKLY;
pattern.interval = 1;
recurrence.pattern = pattern;
RecurrenceRange range = new RecurrenceRange();
range.type = RecurrenceRangeType.NO_END;
range.startDate = new DateOnly(1900,1,1);
recurrence.range = range;
settings.recurrence = recurrence;
accessReviewScheduleDefinition.settings = settings;

graphClient.identityGovernance().accessReviews().definitions()
    .buildRequest()
    .post(accessReviewScheduleDefinition);

```