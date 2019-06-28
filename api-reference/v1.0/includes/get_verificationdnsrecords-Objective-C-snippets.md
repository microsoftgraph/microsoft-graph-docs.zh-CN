---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fbb6148143942f3798bc17d91839c6af96b82a25
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35323191"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/domains/{domain-name}/verificationDnsRecords"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *domainDnsRecordList = [[NSMutableArray alloc] init];
        domainDnsRecordList = [jsonFinal valueForKey:@"value"];
        MSGraphDomainDnsRecord *domainDnsRecord = [[MSGraphDomainDnsRecord alloc] initWithDictionary:[domainDnsRecordList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```