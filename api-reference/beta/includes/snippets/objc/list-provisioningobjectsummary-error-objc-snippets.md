---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e4255edf3ff97d02dac7f0de09e1a91cb99091a1
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35719993"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/auditLogs/directoryProvisioning"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *provisioningObjectSummaryList = [[NSMutableArray alloc] init];
        provisioningObjectSummaryList = [jsonFinal valueForKey:@"value"];
        MSGraphProvisioningObjectSummary *provisioningObjectSummary = [[MSGraphProvisioningObjectSummary alloc] initWithDictionary:[provisioningObjectSummaryList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```