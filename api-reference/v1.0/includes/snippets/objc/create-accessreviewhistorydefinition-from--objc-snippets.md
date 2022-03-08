---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f04d25a7eeb1d2413ece274204239db1ee9820b
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337656"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identityGovernance/accessReviews/historyDefinitions"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAccessReviewHistoryDefinition *accessReviewHistoryDefinition = [[MSGraphAccessReviewHistoryDefinition alloc] init];
[accessReviewHistoryDefinition setDisplayName:@"Last quarter's group reviews April 2021"];
NSMutableArray *decisionsList = [[NSMutableArray alloc] init];
[decisionsList addObject: @"approve"];
[decisionsList addObject: @"deny"];
[decisionsList addObject: @"dontKnow"];
[decisionsList addObject: @"notReviewed"];
[decisionsList addObject: @"notNotified"];
[accessReviewHistoryDefinition setDecisions:decisionsList];
MSGraphAccessReviewHistoryScheduleSettings *scheduleSettings = [[MSGraphAccessReviewHistoryScheduleSettings alloc] init];
[scheduleSettings setReportRange:@"P1M"];
MSGraphPatternedRecurrence *recurrence = [[MSGraphPatternedRecurrence alloc] init];
MSGraphRecurrencePattern *pattern = [[MSGraphRecurrencePattern alloc] init];
[pattern setType: [MSGraphRecurrencePatternType daily]];
[pattern setInterval: 1];
[recurrence setPattern:pattern];
MSGraphRecurrenceRange *range = [[MSGraphRecurrenceRange alloc] init];
[range setType: [MSGraphRecurrenceRangeType noEnd]];
[range setStartDate: "2018-08-03T21:02:30.667Z"];
[range setCount: 0];
[recurrence setRange:range];
[scheduleSettings setRecurrence:recurrence];
[accessReviewHistoryDefinition setScheduleSettings:scheduleSettings];
NSMutableArray *scopesList = [[NSMutableArray alloc] init];
MSGraphAccessReviewScope *scopes = [[MSGraphAccessReviewScope alloc] init];
[scopes setQueryType:@"MicrosoftGraph"];
[scopes setQuery:@"/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, 'accessPackageAssignments')"];
[scopes setQueryRoot: null];
[scopesList addObject: scopes];
MSGraphAccessReviewScope *scopes = [[MSGraphAccessReviewScope alloc] init];
[scopes setQueryType:@"MicrosoftGraph"];
[scopes setQuery:@"/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups')"];
[scopes setQueryRoot: null];
[scopesList addObject: scopes];
[accessReviewHistoryDefinition setScopes:scopesList];

NSError *error;
NSData *accessReviewHistoryDefinitionData = [accessReviewHistoryDefinition getSerializedDataWithError:&error];
[urlRequest setHTTPBody:accessReviewHistoryDefinitionData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```