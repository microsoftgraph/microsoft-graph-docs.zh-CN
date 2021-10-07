---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8934f6c691592d5ee283820aa5dea68cc73670915ce7b2ba802814d440eef915
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104801"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/education/classes/11021/assignments/19002"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphEducationAssignment *educationAssignment = [[MSGraphEducationAssignment alloc] init];
[educationAssignment setDisplayName:@"Week 1 reading assignment"];
MSGraphEducationItemBody *instructions = [[MSGraphEducationItemBody alloc] init];
[instructions setContentType: [MSGraphBodyType text]];
[instructions setContent:@"Read chapters 1 through 3"];
[educationAssignment setInstructions:instructions];
[educationAssignment setDueDateTime: "2014-02-01T00:00:00Z"];
[educationAssignment setAddedStudentAction: [MSGraphEducationAddedStudentAction none]];
[educationAssignment setAddToCalendarAction: [MSGraphEducationAddToCalendarOptions studentsAndPublisher]];

NSError *error;
NSData *educationAssignmentData = [educationAssignment getSerializedDataWithError:&error];
[urlRequest setHTTPBody:educationAssignmentData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```