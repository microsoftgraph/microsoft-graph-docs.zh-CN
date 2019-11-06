---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 036c9b567bfb65b227ebf9f0668176e016fd5c7c
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997989"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/profile/educationalActivities"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *educationalActivityList = [[NSMutableArray alloc] init];
        educationalActivityList = [jsonFinal valueForKey:@"value"];
        MSGraphEducationalActivity *educationalActivity = [[MSGraphEducationalActivity alloc] initWithDictionary:[educationalActivityList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```