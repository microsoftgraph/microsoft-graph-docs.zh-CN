---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1ba818c0203856a9f6383db833b6540b14771317
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706836"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/auditLogs/directoryAudits"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *directoryAuditList = [[NSMutableArray alloc] init];
        directoryAuditList = [jsonFinal valueForKey:@"value"];
        MSGraphDirectoryAudit *directoryAudit = [[MSGraphDirectoryAudit alloc] initWithDictionary:[directoryAuditList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```