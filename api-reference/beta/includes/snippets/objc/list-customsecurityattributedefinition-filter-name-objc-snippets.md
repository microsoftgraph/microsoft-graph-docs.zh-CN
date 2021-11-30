---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b381da8ebf64fc7e64eecede164382e8b50cc17f
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61224633"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/directory/customSecurityAttributeDefinitions?$filter=name%20eq%20'Project'%20and%20status%20eq%20'Available'"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        MSCollection *collection = [[MSCollection alloc] initWithData:data error:&jsonError];
        MSGraphCustomSecurityAttributeDefinition *customSecurityAttributeDefinition = [[MSGraphCustomSecurityAttributeDefinition alloc] initWithDictionary:[[collection value] objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```