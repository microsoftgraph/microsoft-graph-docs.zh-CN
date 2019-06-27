---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 50521d7c104479d965b402a078a61c75cd70fd6d
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35330796"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getMailboxUsageMailboxCounts(period='D7')?$format=text/csv"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *mailboxUsageMailboxCountsList = [[NSMutableArray alloc] init];
        mailboxUsageMailboxCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphMailboxUsageMailboxCounts *mailboxUsageMailboxCounts = [[MSGraphMailboxUsageMailboxCounts alloc] initWithDictionary:[mailboxUsageMailboxCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```