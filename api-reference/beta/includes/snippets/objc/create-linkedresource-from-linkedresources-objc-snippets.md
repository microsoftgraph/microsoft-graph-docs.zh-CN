---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 81d9cb249b0d6bcaf52bad5fdd2a61f48e0c50af
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2020
ms.locfileid: "48375689"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphLinkedResource *linkedResource = [[MSGraphLinkedResource alloc] init];
[linkedResource setWebUrl:@"https://microsoft.com"];
[linkedResource setApplicationName:@"Microsoft"];
[linkedResource setDisplayName:@"Microsoft"];
[linkedResource setExternalId:@"dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9"];

NSError *error;
NSData *linkedResourceData = [linkedResource getSerializedDataWithError:&error];
[urlRequest setHTTPBody:linkedResourceData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```