---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e89e1cc6a080a9448af544b3b13bb875fffd3c64
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724315"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/findRoomLists"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *emailAddressList = [[NSMutableArray alloc] init];
        emailAddressList = [jsonFinal valueForKey:@"value"];
        MSGraphEmailAddress *emailAddress = [[MSGraphEmailAddress alloc] initWithDictionary:[emailAddressList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```