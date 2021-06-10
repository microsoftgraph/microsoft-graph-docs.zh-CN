---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3e734df7e0bd5e6deb41e4500975a592b3f27a3f
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52871468"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/education/classes/{id}/assignmentDefaults"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphEducationAssignmentDefaults *educationAssignmentDefaults = [[MSGraphEducationAssignmentDefaults alloc] init];
[educationAssignmentDefaults setAddedStudentAction: [MSGraphEducationAddedStudentAction assignIfOpen]];
[educationAssignmentDefaults setAddToCalendarAction: [MSGraphEducationAddToCalendarOptions studentsAndTeamOwners]];
[educationAssignmentDefaults setNotificationChannelUrl:@"https://graph.microsoft.com/beta/teams('id')/channels('id')"];

NSError *error;
NSData *educationAssignmentDefaultsData = [educationAssignmentDefaults getSerializedDataWithError:&error];
[urlRequest setHTTPBody:educationAssignmentDefaultsData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```