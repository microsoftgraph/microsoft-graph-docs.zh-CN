---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 112db73fe400e81c12ca5b73817a05541b7b40fea75596fd0c97d07e0fa99c34
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279193"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/education/classes/8ddcac47-0b45-4cdb-b10a-d36a07a3dd62/assignments"]]];
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