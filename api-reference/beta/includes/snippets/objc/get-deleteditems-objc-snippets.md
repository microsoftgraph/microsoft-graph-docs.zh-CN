---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2d5f7101ff48f9da504e0ed029cf4e4e1f1f705d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35521326"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/directory/deleteditems/microsoft.graph.group"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *groupList = [[NSMutableArray alloc] init];
        groupList = [jsonFinal valueForKey:@"value"];
        MSGraphGroup *group = [[MSGraphGroup alloc] initWithDictionary:[groupList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```