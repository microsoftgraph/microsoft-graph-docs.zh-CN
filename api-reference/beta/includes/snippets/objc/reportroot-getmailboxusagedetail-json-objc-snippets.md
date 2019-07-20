---
description: 自动生成的文件。 不修改
ms.openlocfilehash: eb3efe1b89e1722f0037390078b034668324e96b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35719552"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getMailboxUsageDetail(period='D7')?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *mailboxUsageDetailList = [[NSMutableArray alloc] init];
        mailboxUsageDetailList = [jsonFinal valueForKey:@"value"];
        MSGraphMailboxUsageDetail *mailboxUsageDetail = [[MSGraphMailboxUsageDetail alloc] initWithDictionary:[mailboxUsageDetailList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```