---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c1797b1476cba76c163963fc44aab3790ad62918
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520747"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/applicationTemplates"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *applicationTemplateList = [[NSMutableArray alloc] init];
        applicationTemplateList = [jsonFinal valueForKey:@"value"];
        MSGraphApplicationTemplate *applicationTemplate = [[MSGraphApplicationTemplate alloc] initWithDictionary:[applicationTemplateList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```