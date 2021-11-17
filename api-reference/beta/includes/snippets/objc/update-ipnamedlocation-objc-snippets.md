---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ad755c5da113514211c41073f4b59d2ce65fb93ae618d877d6c41eed1b8d759
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332394"
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