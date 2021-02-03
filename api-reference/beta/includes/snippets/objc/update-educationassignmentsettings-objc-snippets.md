---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e5bb867d4f7ec30625f1f0fa1b8b1621dc94c7c4
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2021
ms.locfileid: "50092493"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/education/classes/{id}/assignmentSettings"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphEducationAssignmentSettings *educationAssignmentSettings = [[MSGraphEducationAssignmentSettings alloc] init];
[educationAssignmentSettings setSubmissionAnimationDisabled: true];

NSError *error;
NSData *educationAssignmentSettingsData = [educationAssignmentSettings getSerializedDataWithError:&error];
[urlRequest setHTTPBody:educationAssignmentSettingsData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```