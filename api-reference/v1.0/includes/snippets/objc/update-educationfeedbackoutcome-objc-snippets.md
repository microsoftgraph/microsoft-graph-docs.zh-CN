---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3abb8cbe24372b7dcb60199566135fcc3e0d4c53124765e7dd2550dd86938d0b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278588"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/submissions/d1bee293-d8bb-48d4-af3e-c8cb0e3c7fe7/outcomes/9c0f2850-ff8f-4fd6-b3ac-e23077b59141"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphEducationOutcome *educationOutcome = [[MSGraphEducationOutcome alloc] init];
MSGraphEducationFeedback *feedback = [[MSGraphEducationFeedback alloc] init];
MSGraphEducationItemBody *text = [[MSGraphEducationItemBody alloc] init];
[text setContent:@"This is feedback for the assignment as a whole."];
[text setContentType: [MSGraphBodyType text]];
[feedback setText:text];
[educationOutcome setFeedback:feedback];

NSError *error;
NSData *educationOutcomeData = [educationOutcome getSerializedDataWithError:&error];
[urlRequest setHTTPBody:educationOutcomeData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```