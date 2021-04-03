---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec8346c79ba4a5adc1f8906b6445d7f32df14890
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51509175"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/policies/adminConsentRequestPolicy"]]];
[urlRequest setHTTPMethod:@"PUT"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAdminConsentRequestPolicy *adminConsentRequestPolicy = [[MSGraphAdminConsentRequestPolicy alloc] init];
[adminConsentRequestPolicy setIsEnabled: true];
[adminConsentRequestPolicy setNotifyReviewers: true];
[adminConsentRequestPolicy setRemindersEnabled: true];
[adminConsentRequestPolicy setRequestDurationInDays: 5];
NSMutableArray *reviewersList = [[NSMutableArray alloc] init];
MSGraphAccessReviewReviewerScope *reviewers = [[MSGraphAccessReviewReviewerScope alloc] init];
[reviewers setQuery:@"/users/b6879be8-fb87-4482-a72e-18445d2b5c54"];
[reviewers setQueryType:@"MicrosoftGraph"];
[reviewersList addObject: reviewers];
MSGraphAccessReviewReviewerScope *reviewers = [[MSGraphAccessReviewReviewerScope alloc] init];
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