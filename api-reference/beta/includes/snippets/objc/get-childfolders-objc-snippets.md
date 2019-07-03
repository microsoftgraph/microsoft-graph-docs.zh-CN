---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f91582d4afc1c32a2b0cfcb2e4387a32ae670649
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35521624"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/mailFolders/AAMkAGVmMDEzM/childFolders"]]];
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