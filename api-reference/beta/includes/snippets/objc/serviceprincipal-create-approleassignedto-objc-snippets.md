---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 76b34bf0f7453ff9c7bf80409c6b1af15abb3e26
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807876"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/servicePrincipals/9028d19c-26a9-4809-8e3f-20ff73e2d75e/appRoleAssignedTo"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAppRoleAssignment *appRoleAssignment = [[MSGraphAppRoleAssignment alloc] init];
[appRoleAssignment setPrincipalId:@"33ad69f9-da99-4bed-acd0-3f24235cb296"];
[appRoleAssignment setResourceId:@"9028d19c-26a9-4809-8e3f-20ff73e2d75e"];
[appRoleAssignment setAppRoleId:@"ef7437e6-4f94-4a0a-a110-a439eb2aa8f7"];

NSError *error;
NSData *appRoleAssignmentData = [appRoleAssignment getSerializedDataWithError:&error];
[urlRequest setHTTPBody:appRoleAssignmentData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```