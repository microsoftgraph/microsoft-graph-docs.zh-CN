---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cb48bbd0177f17f83a55bfaaee28c23ccfe161c6
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681768"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identity/conditionalAccess/namedLocations/0854951d-5fc0-4eb1-b392-9b2c9d7949c2"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphNamedLocation *namedLocation = [[MSGraphNamedLocation alloc] init];
[namedLocation setDisplayName:@"Untrusted named location with only IPv4 address"];
[namedLocation setIsTrusted: false];
NSMutableArray *ipRangesList = [[NSMutableArray alloc] init];
MSGraphIpRange *ipRanges = [[MSGraphIpRange alloc] init];
[ipRanges setCidrAddress:@"6.5.4.3/18"];
[ipRangesList addObject: ipRanges];
[namedLocation setIpRanges:ipRangesList];

NSError *error;
NSData *namedLocationData = [namedLocation getSerializedDataWithError:&error];
[urlRequest setHTTPBody:namedLocationData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```