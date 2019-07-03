---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ab70d7866c46080a2aae006af45c5518d66a806f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520088"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/activities"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *itemActivityOLDList = [[NSMutableArray alloc] init];
        itemActivityOLDList = [jsonFinal valueForKey:@"value"];
        MSGraphItemActivityOLD *itemActivityOLD = [[MSGraphItemActivityOLD alloc] initWithDictionary:[itemActivityOLDList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```