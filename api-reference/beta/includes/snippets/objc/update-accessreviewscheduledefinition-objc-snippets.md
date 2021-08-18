---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8ead342c607d71a9841fb107ecf14dd07d894b2a
ms.sourcegitcommit: 22bd45d272681658d46a8b99af3c3eabc7b05cb1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/18/2021
ms.locfileid: "58384067"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identityGovernance/accessReviews/definitions/60860cdd-fb4d-4054-91ba-f75e04444aa6"]]];
[urlRequest setHTTPMethod:@"PUT"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAccessReviewScheduleDefinition *accessReviewScheduleDefinition = [[MSGraphAccessReviewScheduleDefinition alloc] init];
[accessReviewScheduleDefinition setId:@"60860cdd-fb4d-4054-91ba-f75e04444aa6"];
[accessReviewScheduleDefinition setDisplayName:@"Test world UPDATED NAME!"];
[accessReviewScheduleDefinition setDescriptionForAdmins:@"Test world"];
[accessReviewScheduleDefinition setDescriptionForReviewers:@"Test world"];
MSGraphAccessReviewScope *scope = [[MSGraphAccessReviewScope alloc] init];
[scope setQuery:@"/groups/b7a059cb-038a-4802-8fc9-b9d1ed0cf11f/transitiveMembers"];
[scope setQueryType:@"MicrosoftGraph"];
[accessReviewScheduleDefinition setScope:scope];
MSGraphAccessReviewScope *instanceEnumerationScope = [[MSGraphAccessReviewScope alloc] init];
[instanceEnumerationScope setQuery:@"/groups/b7a059cb-038a-4802-8fc9-b9d1ed0cf11f"];
[instanceEnumerationScope setQueryType:@"MicrosoftGraph"];
[accessReviewScheduleDefinition setInstanceEnumerationScope:instanceEnumerationScope];
NSMutableArray *reviewersList = [[NSMutableArray alloc] init];
[accessReviewScheduleDefinition setReviewers:reviewersList];
MSGraphAccessReviewScheduleSettings *settings = [[MSGraphAccessReviewScheduleSettings alloc] init];
[settings setMailNotificationsEnabled: true];
[settings setReminderNotificationsEnabled: true];
[settings setJustificationRequiredOnApproval: true];
[settings setDefaultDecisionEnabled: false];
[settings setDefaultDecision:@"None"];
[settings setInstanceDurationInDays: 3];
[settings setAutoApplyDecisionsEnabled: false];
[settings setRecommendationsEnabled: true];
MSGraphPatternedRecurrence *recurrence = [[MSGraphPatternedRecurrence alloc] init];
MSGraphRecurrencePattern *pattern = [[MSGraphRecurrencePattern alloc] init];
[pattern setType: [MSGraphRecurrencePatternType weekly]];
[pattern setInterval: 1];
[recurrence setPattern:pattern];
MSGraphRecurrenceRange *range = [[MSGraphRecurrenceRange alloc] init];
[range setType: [MSGraphRecurrenceRangeType noEnd]];
[range setStartDate:@"2020-09-15"];
[recurrence setRange:range];
[settings setRecurrence:recurrence];
[accessReviewScheduleDefinition setSettings:settings];

NSError *error;
NSData *accessReviewScheduleDefinitionData = [accessReviewScheduleDefinition getSerializedDataWithError:&error];
[urlRequest setHTTPBody:accessReviewScheduleDefinitionData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```