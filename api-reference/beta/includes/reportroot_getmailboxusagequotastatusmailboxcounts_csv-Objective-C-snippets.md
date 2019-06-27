---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 13b54fc0436d0bde7f85fcab58d8e0bd8c91919f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35315549"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getMailboxUsageQuotaStatusMailboxCounts(period='D7')?$format=text/csv"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *mailboxUsageQuotaStatusMailboxCountsList = [[NSMutableArray alloc] init];
        mailboxUsageQuotaStatusMailboxCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphMailboxUsageQuotaStatusMailboxCounts *mailboxUsageQuotaStatusMailboxCounts = [[MSGraphMailboxUsageQuotaStatusMailboxCounts alloc] initWithDictionary:[mailboxUsageQuotaStatusMailboxCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```