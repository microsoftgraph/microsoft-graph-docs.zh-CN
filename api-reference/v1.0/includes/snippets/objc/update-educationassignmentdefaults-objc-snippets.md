---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8634b211616d6430d0191d99c7467ee5f5efe5be463683d6a92bbd0709c91b36
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333966"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentDefaults"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphEducationAssignmentDefaults *educationAssignmentDefaults = [[MSGraphEducationAssignmentDefaults alloc] init];
[educationAssignmentDefaults setAddedStudentAction: [MSGraphEducationAddedStudentAction assignIfOpen]];
[educationAssignmentDefaults setNotificationChannelUrl:@"https://graph.microsoft.com/beta/teams('acdefc6b-2dc6-4e71-b1e9-6d9810ab1793')/channels('3da03fc4-8eac-4459-84fb-1422dc01f65e')"];

NSError *error;
NSData *educationAssignmentDefaultsData = [educationAssignmentDefaults getSerializedDataWithError:&error];
[urlRequest setHTTPBody:educationAssignmentDefaultsData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```