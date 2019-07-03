---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1400eb1c0b9270bc6758ec47eaf97d99139ce8bd
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520326"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getOffice365ActivationsUserDetail?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *office365ActivationsUserDetailList = [[NSMutableArray alloc] init];
        office365ActivationsUserDetailList = [jsonFinal valueForKey:@"value"];
        MSGraphOffice365ActivationsUserDetail *office365ActivationsUserDetail = [[MSGraphOffice365ActivationsUserDetail alloc] initWithDictionary:[office365ActivationsUserDetailList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```