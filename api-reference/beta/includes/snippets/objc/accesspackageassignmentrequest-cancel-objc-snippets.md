---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fc943739c3eeed902343f7128f93ed5c7d1991637cd03033fb876c7bedbb5e36
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902802"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}/cancel"]]];
[urlRequest setHTTPMethod:@"POST"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSString *id = @"request-id";
payloadDictionary[@"id"] = id;

NSString *requestStatus = @"cancelled";
payloadDictionary[@"requestStatus"] = requestStatus;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```