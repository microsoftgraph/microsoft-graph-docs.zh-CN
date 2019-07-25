---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6cc16a37a811193c8c05cb0c7510e7f0b7b7b8de
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724112"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/mailFolders"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *mailFolderList = [[NSMutableArray alloc] init];
        mailFolderList = [jsonFinal valueForKey:@"value"];
        MSGraphMailFolder *mailFolder = [[MSGraphMailFolder alloc] initWithDictionary:[mailFolderList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```