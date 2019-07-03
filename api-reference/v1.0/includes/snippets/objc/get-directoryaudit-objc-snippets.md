---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0de6d22d2de42aeb2e00162a35300dea26c1d79e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35509900"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
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