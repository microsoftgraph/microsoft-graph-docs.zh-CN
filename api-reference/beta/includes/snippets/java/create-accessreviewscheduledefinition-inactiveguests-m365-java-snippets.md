---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e0ab6b4c70734c0ac40bbdde76c4a41ca6f888ab9d1d549adef28a187d86dd40
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104113"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewScheduleDefinition accessReviewScheduleDefinition = new AccessReviewScheduleDefinition();
accessReviewScheduleDefinition.displayName = "Review inactive guests on teams";
accessReviewScheduleDefinition.descriptionForAdmins = "Control guest user access to our teams.";
accessReviewScheduleDefinition.descriptionForReviewers = "Information security is everyone's responsibility. Review our access policy for more.";
AccessReviewQueryScope instanceEnumerationScope = new AccessReviewQueryScope();
instanceEnumerationScope.query = "/groups?$filter=(groupTypes/any(c:c+eq+'Unified') and resourceProvisioningOptions/Any(x:x eq 'Team')')";
instanceEnumerationScope.queryType = "MicrosoftGraph";
accessReviewScheduleDefinition.instanceEnumerationScope = instanceEnumerationScope;
AccessReviewInactiveUsersQueryScope scope = new AccessReviewInactiveUsersQueryScope();
scope.query = "./members/microsoft.graph.user/?$filter=(userType eq 'Guest')";
scope.queryType = "MicrosoftGraph";
scope.inactiveDuration = DatatypeFactory.newInstance().newDuration("P30D");
accessReviewScheduleDefinition.scope = scope;
LinkedList<AccessReviewReviewerScope> reviewersList = new LinkedList<AccessReviewReviewerScope>();
AccessReviewReviewerScope reviewers = new AccessReviewReviewerScope();
reviewers.query = "./owners";
reviewers.queryType = "MicrosoftGraph";
reviewersList.add(reviewers);
accessReviewScheduleDefinition.reviewers = reviewersList;
LinkedList<AccessReviewReviewerScope> fallbackReviewersList = new LinkedList<AccessReviewReviewerScope>();
AccessReviewReviewerScope fallbackReviewers = new AccessReviewReviewerScope();
fallbackReviewers.query = "/users/fc9a2c2b-1ddc-486d-a211-5fe8ca77fa1f";
fallbackReviewers.queryType = "MicrosoftGraph";
fallbackReviewersList.add(fallbackReviewers);
accessReviewScheduleDefinition.fallbackReviewers = fallbackReviewersList;
AccessReviewScheduleSettings settings = new AccessReviewScheduleSettings();
settings.mailNotificationsEnabled = true;
settings.reminderNotificationsEnabled = true;
settings.justificationRequiredOnApproval = true;
settings.recommendationsEnabled = true;
settings.instanceDurationInDays = 3;
PatternedRecurrence recurrence = new PatternedRecurrence();
RecurrencePattern pattern = new RecurrencePattern();
pattern.type = RecurrencePatternType.ABSOLUTE_MONTHLY;
pattern.dayOfMonth = 5;
pattern.interval = 3;
recurrence.pattern = pattern;
RecurrenceRange range = new RecurrenceRange();
range.type = RecurrenceRangeType.NO_END;
range.startDate = new DateOnly(1900,1,1);
recurrence.range = range;
settings.recurrence = recurrence;
settings.defaultDecisionEnabled = true;
settings.defaultDecision = "Deny";
settings.autoApplyDecisionsEnabled = true;
accessReviewScheduleDefinition.settings = settings;

graphClient.identityGovernance().accessReviews().definitions()
    .buildRequest()
    .post(accessReviewScheduleDefinition);

```