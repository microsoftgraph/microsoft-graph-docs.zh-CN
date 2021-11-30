---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1ab80264d9dd06dc57a98a2e761b5b055c3acf0d
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61226502"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/directory/attributeSets"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAttributeSet *attributeSet = [[MSGraphAttributeSet alloc] init];
[attributeSet setId:@"Engineering"];
[attributeSet setDescription:@"Attributes for engineering team"];
[attributeSet setMaxAttributesPerSet: 25];

NSError *error;
NSData *attributeSetData = [attributeSet getSerializedDataWithError:&error];
[urlRequest setHTTPBody:attributeSetData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```