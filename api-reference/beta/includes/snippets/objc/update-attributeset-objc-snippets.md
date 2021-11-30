---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f396d26ade7da1e8f58bd8d65e636008ed8690ef
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61223550"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/directory/attributeSets/Engineering"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAttributeSet *attributeSet = [[MSGraphAttributeSet alloc] init];
[attributeSet setDescription:@"Attributes for engineering team"];
[attributeSet setMaxAttributesPerSet: 20];

NSError *error;
NSData *attributeSetData = [attributeSet getSerializedDataWithError:&error];
[urlRequest setHTTPBody:attributeSetData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```