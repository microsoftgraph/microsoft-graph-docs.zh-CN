---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7f87d1fd995e3d6856409489ec8b1ca456f6fe0b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35715454"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/education/classes/{class-id}/teachers"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *educationUserList = [[NSMutableArray alloc] init];
        educationUserList = [jsonFinal valueForKey:@"value"];
        MSGraphEducationUser *educationUser = [[MSGraphEducationUser alloc] initWithDictionary:[educationUserList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```