---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6466eadb82ce18cc9516ae33528b5c7a9adf8d04
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52473980"
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