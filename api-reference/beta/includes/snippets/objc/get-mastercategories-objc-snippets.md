---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0b781da3d78ed31326233335517573ce71587b91
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35519823"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/outlook/masterCategories"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *outlookCategoryList = [[NSMutableArray alloc] init];
        outlookCategoryList = [jsonFinal valueForKey:@"value"];
        MSGraphOutlookCategory *outlookCategory = [[MSGraphOutlookCategory alloc] initWithDictionary:[outlookCategoryList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```