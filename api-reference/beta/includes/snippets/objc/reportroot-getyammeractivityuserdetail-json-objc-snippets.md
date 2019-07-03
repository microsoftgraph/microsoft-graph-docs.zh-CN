---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 456dcf98629bffc62bfb38009f13c1bbfc70e602
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35500313"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getYammerActivityUserDetail(period='D7')?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *yammerActivityUserDetailList = [[NSMutableArray alloc] init];
        yammerActivityUserDetailList = [jsonFinal valueForKey:@"value"];
        MSGraphYammerActivityUserDetail *yammerActivityUserDetail = [[MSGraphYammerActivityUserDetail alloc] initWithDictionary:[yammerActivityUserDetailList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```