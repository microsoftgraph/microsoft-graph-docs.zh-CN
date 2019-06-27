---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f9b88e624db1a8fe82b5b3f0f6583e8360a42a20
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35330666"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/groups/{id}/conversations/{id}/threads"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *conversationThreadList = [[NSMutableArray alloc] init];
        conversationThreadList = [jsonFinal valueForKey:@"value"];
        MSGraphConversationThread *conversationThread = [[MSGraphConversationThread alloc] initWithDictionary:[conversationThreadList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```