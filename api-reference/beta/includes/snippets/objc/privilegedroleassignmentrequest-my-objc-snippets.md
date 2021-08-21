---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 99eb75d3a369b6a90c9b869913962eeb50d968d42521e9ae221820c6b211910e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219710"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/privilegedRoleAssignmentRequests/my"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        MSCollection *collection = [[MSCollection alloc] initWithData:data error:&jsonError];
        MSGraphPrivilegedRoleAssignmentRequest *privilegedRoleAssignmentRequest = [[MSGraphPrivilegedRoleAssignmentRequest alloc] initWithDictionary:[[collection value] objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```