---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 66808a620728644b48b27be8030dcaf3cd525cd9
ms.sourcegitcommit: 22bd45d272681658d46a8b99af3c3eabc7b05cb1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/18/2021
ms.locfileid: "58384376"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/education/classes/8b8cec7f-d0d8-4974-982a-e29396ddbe7f/assignments"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphEducationAssignment *educationAssignment = [[MSGraphEducationAssignment alloc] init];
[educationAssignment setDueDateTime: "2014-02-01T00:00:00Z"];
[educationAssignment setDisplayName:@"Midterm 1"];
MSGraphEducationItemBody *instructions = [[MSGraphEducationItemBody alloc] init];
[instructions setContentType: [MSGraphBodyType text]];
[instructions setContent:@"Read chapters 1 through 3"];
[educationAssignment setInstructions:instructions];
MSGraphEducationAssignmentGradeType *grading = [[MSGraphEducationAssignmentGradeType alloc] init];
[grading setMaxPoints: 100];
[educationAssignment setGrading:grading];
MSGraphEducationAssignmentRecipient *assignTo = [[MSGraphEducationAssignmentRecipient alloc] init];
[educationAssignment setAssignTo:assignTo];
[educationAssignment setStatus: [MSGraphEducationAssignmentStatus draft]];
[educationAssignment setAllowStudentsToAddResourcesToSubmission: true];

NSError *error;
NSData *educationAssignmentData = [educationAssignment getSerializedDataWithError:&error];
[urlRequest setHTTPBody:educationAssignmentData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```