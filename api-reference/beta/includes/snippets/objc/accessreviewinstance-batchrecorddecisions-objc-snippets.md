---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 19dcf16e36d15dcb16585e8c3e59fbc5a60aa4d58a7c0c3e3634e27e4a958128
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104147"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/pendingAccessReviewInstances/{accessReviewInstanceId}/batchRecordDecisions"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSString *decision = @"Approve";
payloadDictionary[@"decision"] = decision;

NSString *justification = @"All principals with access need continued access to the resource (Marketing Group) as all the principals are on the marketing team";
payloadDictionary[@"justification"] = justification;

NSString *resourceId = @"a5c51e59-3fcd-4a37-87a1-835c0c21488a";
payloadDictionary[@"resourceId"] = resourceId;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```