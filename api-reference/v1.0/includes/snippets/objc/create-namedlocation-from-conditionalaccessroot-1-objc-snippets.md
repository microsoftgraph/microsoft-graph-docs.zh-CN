---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0f0513c2f21876232dae429056d546c4a475808badb4da462922a46449be869e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333157"
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