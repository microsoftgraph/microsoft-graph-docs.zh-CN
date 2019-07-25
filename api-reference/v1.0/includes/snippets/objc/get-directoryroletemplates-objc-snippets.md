---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b032a8a6052857eb4f6d8f1bd29189137604790e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35733570"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/directoryRoleTemplates"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *directoryRoleTemplateList = [[NSMutableArray alloc] init];
        directoryRoleTemplateList = [jsonFinal valueForKey:@"value"];
        MSGraphDirectoryRoleTemplate *directoryRoleTemplate = [[MSGraphDirectoryRoleTemplate alloc] initWithDictionary:[directoryRoleTemplateList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```