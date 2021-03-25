---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: af0f461bb64c7bc2f3ea8217fd0e86550e01a49e
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201457"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/policies/adminConsentRequestPolicy"]]];
[urlRequest setHTTPMethod:@"PUT"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAdminConsentRequestPolicy *adminConsentRequestPolicy = [[MSGraphAdminConsentRequestPolicy alloc] init];
[adminConsentRequestPolicy setIsEnabled: true];
[adminConsentRequestPolicy setNotifyReviewers: true];
[adminConsentRequestPolicy setRemindersEnabled: true];
[adminConsentRequestPolicy setRequestDurationInDays: 5];
NSMutableArray *reviewersList = [[NSMutableArray alloc] init];
MSGraphAccessReviewScope *reviewers = [[MSGraphAccessReviewScope alloc] init];
[reviewers setQuery:@"/users/b6879be8-fb87-4482-a72e-18445d2b5c54"];
[reviewers setQueryType:@"MicrosoftGraph"];
[reviewersList addObject: reviewers];
MSGraphAccessReviewScope *reviewers = [[MSGraphAccessReviewScope alloc] init];
[reviewers setQuery:@"/users/b3427cc5-bf69-4dcd-95f7-ed1eb432f5e9"];
[reviewers setQueryType:@"MicrosoftGraph"];
[reviewersList addObject: reviewers];
[adminConsentRequestPolicy setReviewers:reviewersList];

NSError *error;
NSData *adminConsentRequestPolicyData = [adminConsentRequestPolicy getSerializedDataWithError:&error];
[urlRequest setHTTPBody:adminConsentRequestPolicyData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```