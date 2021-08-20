---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9bed1178e0d3968a686149ce3736816bf77b7eba57e5d0e86f29ad5de3746303
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218570"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/education/classes/{id}/assignments/{id}/submissions/{id}/outcomes/{id}"]]];
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