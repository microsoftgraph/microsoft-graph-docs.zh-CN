---
description: 自动生成的文件。 不修改
ms.openlocfilehash: aad8d04e37f3c6718e057f49b85afe8b85281f67
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35521527"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/events?$select=subject,body,bodyPreview"]]];
[urlRequest setHTTPMethod:@"GET"];
[urlRequest setValue:@"outlook.body-content-type=\"text\"" forHTTPHeaderField:@"Prefer"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *eventList = [[NSMutableArray alloc] init];
        eventList = [jsonFinal valueForKey:@"value"];
        MSGraphEvent *event = [[MSGraphEvent alloc] initWithDictionary:[eventList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```