---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 488d88a3fa35999d3921d7f062bb4a688b1bccb4
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35478901"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/directoryRoles/delta"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *directoryRoleList = [[NSMutableArray alloc] init];
        directoryRoleList = [jsonFinal valueForKey:@"value"];
        MSGraphDirectoryRole *directoryRole = [[MSGraphDirectoryRole alloc] initWithDictionary:[directoryRoleList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```