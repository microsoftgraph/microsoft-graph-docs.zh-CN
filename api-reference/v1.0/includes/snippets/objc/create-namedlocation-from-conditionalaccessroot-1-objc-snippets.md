---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 061d8b0aa9ceda1d234eb992b697da2a86208b1e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963968"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identity/conditionalAccess/namedLocations"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphNamedLocation *namedLocation = [[MSGraphNamedLocation alloc] init];
[namedLocation setDisplayName:@"Untrusted IP named location"];
[namedLocation setIsTrusted: false];
NSMutableArray *ipRangesList = [[NSMutableArray alloc] init];
MSGraphIpRange *ipRanges = [[MSGraphIpRange alloc] init];
[ipRanges setCidrAddress:@"12.34.221.11/22"];
[ipRangesList addObject: ipRanges];
MSGraphIpRange *ipRanges = [[MSGraphIpRange alloc] init];
[ipRanges setCidrAddress:@"2001:0:9d38:90d6:0:0:0:0/63"];
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