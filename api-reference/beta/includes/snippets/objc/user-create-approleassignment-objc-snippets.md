---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c1e6eb4842b1b091413f786cf78f524605e0f0c8946a9bb2781a443f85e955a8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378548"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/users/cde330e5-2150-4c11-9c5b-14bfdc948c79/appRoleAssignments"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAppRoleAssignment *appRoleAssignment = [[MSGraphAppRoleAssignment alloc] init];
[appRoleAssignment setPrincipalId:@"cde330e5-2150-4c11-9c5b-14bfdc948c79"];
[appRoleAssignment setResourceId:@"8e881353-1735-45af-af21-ee1344582a4d"];
[appRoleAssignment setAppRoleId:@"00000000-0000-0000-0000-000000000000"];

NSError *error;
NSData *appRoleAssignmentData = [appRoleAssignment getSerializedDataWithError:&error];
[urlRequest setHTTPBody:appRoleAssignmentData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```