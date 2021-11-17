---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: badd87a0b781bf34a2840d650aae8ceaf8bb57747989e5f52106503f5f46827f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161885"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/sourcecollections/1a9b4145d8f84e39bc45a7f68c5c5119?$expand=addToReviewSetOperation,custodianSources,lastEstimateStatisticsOperation"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphSourceCollection *sourceCollection = [[MSGraphSourceCollection alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```