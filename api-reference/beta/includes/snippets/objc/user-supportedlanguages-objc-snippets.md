---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e0c1f17d6b25324075f1d45319cfc173a9a234a1
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35500504"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/outlook/supportedLanguages"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *localeInfoList = [[NSMutableArray alloc] init];
        localeInfoList = [jsonFinal valueForKey:@"value"];
        MSGraphLocaleInfo *localeInfo = [[MSGraphLocaleInfo alloc] initWithDictionary:[localeInfoList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```