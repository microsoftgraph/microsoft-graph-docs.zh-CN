---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8f5157eec4042474be32e3f5d97f799769118d32
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470316"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/education/classes/{id}/assignmentDefaults"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphEducationAssignmentDefaults *educationAssignmentDefaults = [[MSGraphEducationAssignmentDefaults alloc] init];
[educationAssignmentDefaults setAddedStudentAction: [MSGraphEducationAddedStudentAction assignIfOpen]];
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