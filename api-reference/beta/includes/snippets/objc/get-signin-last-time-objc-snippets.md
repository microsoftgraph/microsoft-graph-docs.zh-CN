---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8846cba446af9d0fd4f8e2279e10837e02945529
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37996310"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/users?$select=displayName,userPrincipalName,"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *userList = [[NSMutableArray alloc] init];
        userList = [jsonFinal valueForKey:@"value"];
        MSGraphUser *user = [[MSGraphUser alloc] initWithDictionary:[userList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```