---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fb37f85ca541a910af768528236d62e8642b246b
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61225771"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/directory/customSecurityAttributeDefinitions/Engineering_ProjectDate"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphCustomSecurityAttributeDefinition *customSecurityAttributeDefinition = [[MSGraphCustomSecurityAttributeDefinition alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```