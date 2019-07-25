---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5b89539573e2e98bf7808332c0a5c7432fba9600
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35876755"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/places/bldg2@contoso.com/microsoft.graph.roomlist/rooms"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *roomList = [[NSMutableArray alloc] init];
        roomList = [jsonFinal valueForKey:@"value"];
        MSGraphRoom *room = [[MSGraphRoom alloc] initWithDictionary:[roomList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```