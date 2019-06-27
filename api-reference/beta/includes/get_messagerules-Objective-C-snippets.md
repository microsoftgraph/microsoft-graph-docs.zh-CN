---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6dddf01ef37d62b93e0a2900f18f9de55288bc76
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35330308"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/mailFolders/inbox/messagerules"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *messageRuleList = [[NSMutableArray alloc] init];
        messageRuleList = [jsonFinal valueForKey:@"value"];
        MSGraphMessageRule *messageRule = [[MSGraphMessageRule alloc] initWithDictionary:[messageRuleList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```