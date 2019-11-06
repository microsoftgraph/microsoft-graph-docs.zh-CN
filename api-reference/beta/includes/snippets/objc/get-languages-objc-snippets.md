---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d6007642783a033ffd666159a29c30b9a299ed8f
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37996923"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/profile/languages"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *languageProficiencyList = [[NSMutableArray alloc] init];
        languageProficiencyList = [jsonFinal valueForKey:@"value"];
        MSGraphLanguageProficiency *languageProficiency = [[MSGraphLanguageProficiency alloc] initWithDictionary:[languageProficiencyList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```