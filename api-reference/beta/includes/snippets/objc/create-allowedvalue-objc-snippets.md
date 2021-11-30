---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 43523fc3c784c6ca6284d37f8d577d49c0bcdde7
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61224501"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/directory/customSecurityAttributeDefinitions/Engineering_Project/allowedValues"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAllowedValue *allowedValue = [[MSGraphAllowedValue alloc] init];
[allowedValue setId:@"Alpine"];
[allowedValue setIsActive:@"true"];

NSError *error;
NSData *allowedValueData = [allowedValue getSerializedDataWithError:&error];
[urlRequest setHTTPBody:allowedValueData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```